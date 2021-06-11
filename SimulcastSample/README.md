# SimulcastSample (サイマルキャスト)

このサンプルでは、サイマルキャスト機能を使用する方法を説明しています。 VideoChatSample のコードをベースにしています。

## ビルド環境

サンプルアプリをビルドするには以下の環境が必要です。

- iOS 10.0 以降がインストールされたデバイス (iPhone / iPad どちらにも対応しています)
  - このサンプルアプリはシミュレータでは動作が保証されません。
- Xcode 11.1 以降
  - 本サンプルアプリでは Swift 5.1 を使用しています。
- CocoaPods 1.6.1 以降

## ビルド方法

このサンプルアプリは CocoaPods によって外部フレームワークの管理を行っているため、
まず最初に以下のように `pod install` を実行する必要があります。

```
$ pod install
```

これにより、適切に外部フレームワークがセットアップされます。
本サンプルアプリは、これだけで Xcode 上でビルドが可能な状態になります。

## サンプルアプリの使い方

このサンプルアプリでは、同じクライアントIDに対して最大で12人までが接続し、同時にビデオチャットに参加できます。
それ以上の人数が同時に接続する場合の挙動については保証されません。
実際に配信されていることを確認したい場合には、複数台のデバイスにこのサンプルアプリをインストールするか、
または他の Sora クライアントを用いて同時に接続する必要があります。

三人以上が同じクライアントIDに対して接続されている場合、画面が複数人で分割されます。

自分自身の配信している動画はポップアップで表示されます。

## 実装上の詳細について

実装上の詳細につきましてはサンプルアプリのソースコード上に詳細なコメントを用意してありますので、適時そちらをご確認ください。