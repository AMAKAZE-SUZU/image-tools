# 画像作成ツール

ブラウザだけで使える画像作成ツールです。インストールや登録は不要で、選んだ画像はサーバーに送信されません。

- **メッセージカードメーカー**(`message-card.html`):背景・写真・メッセージ・フォントを選んで、Twitter向けのカード画像を作ります。複数枚のまとめて作成(ZIP保存)にも対応しています。
- **アニメポスターメーカー**(`animated-poster.html`):写真や文字に動きを付け、キラキラや紙吹雪を重ねた動くポスターを、MP4・GIFで保存します。
- **リサイズ・トリミング**(`image-resizer.html`):画像を好きな縦横比で切り抜き、大きさを変えてPNG・JPEG・WebPで保存します。まとめて処理してZIP保存もできます。
- **画像分割**(`image-splitter.html`):1枚の画像をパノラマ・4分割・自由な格子に分けて保存します。まとめて投稿すると大きな1枚の絵のように見せられます。
- **ポスターメーカー**(`poster-maker.html`):レイアウトのテンプレートを作って保存し、画像を差し込んでポスターを作ります。メンバー全員分の一括作成(ZIP保存)にも対応しています。

使い方はトップページ(`index.html`)にまとめています。

更新内容は [CHANGELOG.md](CHANGELOG.md) にまとめています。

## ファイル構成

| ファイル | 内容 |
| --- | --- |
| `index.html` | トップページ(ツール一覧と使い方) |
| `message-card.html` | メッセージカードメーカー |
| `poster-maker.html` | ポスターメーカー |
| `animated-poster.html` | アニメポスターメーカー |
| `image-resizer.html` | リサイズ・トリミング |
| `image-splitter.html` | 画像分割 |
| `CHANGELOG.md` | 更新履歴 |

## 使用しているもの

- フォント:Google Fonts(SIL Open Font License)
- ZIP作成:JSZip(MITライセンス、cdnjsから読み込み)
- MP4の作成:mp4-muxer(MITライセンス、jsDelivrから読み込み)
- GIFの作成:gifenc(MITライセンス、animated-poster.html に組み込み)
- 日本語の文節の判定:BudouX(Google、Apache License 2.0。日本語モデルを message-card.html と animated-poster.html に組み込み)
