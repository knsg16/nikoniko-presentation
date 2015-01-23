NicoNico SPEENYA
====

ブラウザに、ニコニコ動画のように右から左に流れるコメントを表示する、Chrome機能拡張とサーバプログラムです。Likeボタンを押すといいね画像が浮き上がったりします。

主にブラウザを使ったプレゼンテーションで使用すると、視聴者とコミュニケーションがとれて良い感じです。

**注意: 社内で使うために作ったツールで、細かいこと考えてないので、このソースコードのまま一般公開サーバとか作ると大変なことになる気がします。**

[スクリーンキャプチャ動画 (YouTube)](http://youtu.be/M0kr4aONMHQ)

![Screen Shot](screenshot.png)

## 開発動機

社内の会議の所帯が大きくなり一人一人が発言しづらくなってきたので、コミュニケーションを促進するために作りました。エンジニアが使うとそれなりに機能しているようです。

## 動かし方

```bash
$ npm start
```

外部サーバで動かす場合は、`extension/scripts/niconico-script.js`の一番上の方にある接続先URLを変更してビルドしてください。

## 機能拡張のビルド方法

ビルドしたものは`public/speenya.crx`に入っています。

自分でビルドしたい場合は鍵を作って下記を実行。ただし、Chrome機能拡張のURLが変わるのでコードを修正する必要があります。

```bash
$ gem install crxmake
$ ./build-extension.sh
```

## ライセンス
[Apache License 2.0](LICENSE)
