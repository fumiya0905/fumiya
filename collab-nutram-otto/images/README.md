# images

LPが読み込む画像を、このフォルダに置きます。ファイル名を合わせれば自動で表示されます（未設置の間は淡い色の枠が出ます）。

| ファイル名 | 表示場所 | 推奨 |
| --- | --- | --- |
| `mv.jpg` | メインビジュアルの静止画（動画の読み込み前・動画が再生できない環境で表示） | 横長 1920×1080 以上、左上が暗め／単調だと文字が読みやすい |
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
- 商品写真（ブランド紹介・T27〜T29・OTTOカード・5セット）：ショップ（shop.ottoanimal.com）の単品商品ページの画像を、BASEの画像配信URLのまま表示しています。単品ページの画像を差し替えるとURLが変わり、LP側の画像が表示されなくなるので、その場合は `index.html` のURLを更新してください。
- `mv.mp4` / `mv.webm` / `mv.jpg`：アップロードいただいた「ニュートラム×OTTOmv.mp4」をもとに作成（音声なし・軽量化。mp4 3.2MB、webm 1.4MB。静止画は動画の冒頭のコマ）。
