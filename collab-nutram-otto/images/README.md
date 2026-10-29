# images

LPが読み込む画像を、このフォルダに置きます。ファイル名を合わせれば自動で表示されます（未設置の間は淡い色の枠が出ます）。

| ファイル名 | 表示場所 | 推奨 |
| --- | --- | --- |
| `mv.jpg` | 動画の最後のコマ（見出し入り）。動画が再生できない環境・動きを減らす設定の人に表示 | 動画から作成 |
| `mv-poster.jpg` | 動画の読み込み前に表示する最初のコマ | 動画から作成 |
| `mv.mp4` / `mv.webm` | メインビジュアルの動画。あれば自動再生・無音・ループ。動画は切らずに16:9で表示し、見出しは動画の下に出ます | 横長 16:9、5MB以下 |
| `story.jpg` | Our Story 中央 | 4:5 |
| `story-nutram.jpg` / `story-otto.jpg` | ブランド紹介 | 16:9 |
| `merit-1.jpg`〜`merit-3.jpg` | Features の3つの利点 | 4:3 |
| `t27.jpg` / `t28.jpg` / `t29.jpg` | Perfect Pair の各レシピ | 4:3 |
| `feature-otto.jpg` | Perfect Pair の OTTO | 4:3 |
| `step-1.jpg`〜`step-3.jpg` | How to use（円形に切り抜き） | 1:1 |
| `howto.jpg` | How to use 右側 | 3:4 |
| `product-1.jpg`〜`product-5.jpg` | Products（1チキン／2サーモン／3低アレルギー源／4皮膚被毛／5ダイエット） | 1:1 |

拡張子は `.jpg` で揃えてください（`.png` や `.jpeg` だと表示されません）。

## 現在入っている画像
- `story.jpg` `merit-1〜3.jpg` `step-1〜3.jpg` `howto.jpg`：Runway で生成したイメージ写真（実在の商品は写っていません）。実写に差し替える場合は同じ名前で上書きしてください。
- `products/`：ショップ（shop.ottoanimal.com）の単品商品ページの写真を取り込んだもの（Nutram 5種・寄り添うごはん 10種）。ブランド紹介・Perfect Pair・5セットのカードで使用。商品写真を更新したら同じ名前で上書きしてください。
- `mv.mp4` / `mv.webm` / `mv.jpg` / `mv-poster.jpg`：アップロードいただいた「Nutram otto lp mv.mp4」（10秒）をもとに作成（音声なし・1280×720に縮小。webm 0.45MB／mp4 0.75MB。WebMを優先して読み込み、再生できない環境ではMP4）。動画を差し替えるときは、新しい動画をアップロードして依頼してください（4ファイルまとめて作り直します）。

## 軽量化について
画像は表示サイズに合わせて縮小しています（手順写真320px、Features・Our Story 800px、商品写真560px など）。
差し替える場合も、同程度のサイズ・JPEG品質80前後にすると、ページの重さを保てます。
