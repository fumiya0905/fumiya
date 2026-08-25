# LP 引き継ぎ資料

SNS採用ブランディング（OTTO SNS マーケティングチーム「SyncLife」）のランディングページです。

---

## 1. ファイル構成

```
index.html          ページ本体（HTML・CSS・JSすべて含む1ファイル）
images/
  gm.jpg            MESSAGE FROM GM の人物写真
  account-1.jpg     VOICE / RESULTS：@makoto__miyamoto
  account-2.jpg     VOICE / RESULTS：@kazuhito__kouno
  account-3.jpg     VOICE / RESULTS：@shimada.info
```

この2つをそのままサーバーにアップロードすれば表示されます。ビルド作業は不要です。

## 2. 技術仕様

| 項目 | 内容 |
| --- | --- |
| CSS | `index.html` 内の `<style>` に記述（外部CSSなし） |
| JavaScript | 末尾に約20行のみ（スマホのメニュー開閉） |
| 外部依存 | Google Fonts（Noto Sans JP / Barlow Condensed）のみ |
| 画像パス | `images/` への相対パス |
| レスポンシブ | 900px を境にスマホ表示／PC表示が切り替わります |
| 動作確認済み | 320px〜1920px（横スクロールなしを確認） |

## 3. 公開前に設定が必要な箇所

以下は仮の値（`href="#"`）のままです。**公開前に必ず差し替えてください。**

| 場所 | 現在の状態 | 設定するもの |
| --- | --- | --- |
| 最終CTAのLINEボタン | `href="#"` | 公式LINEのURL |
| フッター「プライバシーポリシー」 | `href="#"` | 該当ページのURL |
| フッター「特定商取引法」 | `href="#"` | 該当ページのURL |
| フッター「お問い合わせ」 | `href="#"` | 該当ページのURL |

※ ヘッダー・ドロワー・料金表のボタンはページ内の最終CTAへ飛ぶ設計です（`#cta`）。
   LINEのURLは最終CTAの1箇所を直せば動線が完成します。
   すべてのボタンから直接LINEへ飛ばしたい場合は、`href="#cta"` を同じURLに置き換えてください。

### あわせてご検討ください

- **OGPタグ**（SNSシェア時のサムネイル・タイトル）は未設定です
- **meta description**（検索結果の説明文）は未設定です
- **favicon** は未設定です
- **アクセス解析タグ**（GA4等）は未設置です

## 4. 既存サイトへの組み込み方

### パターンA：独立した1ページとして公開する（推奨）

`/lp/` などのディレクトリに `index.html` と `images/` をそのまま設置してください。
最も手間がかからず、表示崩れも起きません。

### パターンB：CMS（WordPress等）のページに組み込む

1. `<style>〜</style>` の中身をテーマのCSSまたはカスタムCSSへ
2. `<body>` の中身をページ本文へ
3. 末尾の `<script>` をフッターへ
4. `images/` をメディアライブラリへアップロードし、パスを差し替え

**注意点：**

- ページ上部のヘッダーは `position: sticky` で追従します。**既存サイトのヘッダーと二重になる**ため、どちらかを非表示にしてください（このLPのヘッダーを消す場合は `.site-head` と `.fixed-cta` を削除）
- CSSのクラス名が既存サイトと衝突する可能性があります（`.wrap` `.stat` `.plan` など一般的な名前を使用しています）。衝突する場合は全体を `.lp-page` などで囲み、セレクタの先頭に付与してください
- 既存サイトのCSSリセットの影響を受ける場合があります

## 5. セクション構成

上から順に以下の通りです。

1. ヘッダー（追従・スマホはハンバーガーメニュー）
2. ファーストビュー
3. PAIN POINTS — 課題（`#problem`）
4. SOLUTION — 解決策（`#solution`）
5. BEFORE / AFTER
6. PROCESS — 4ステップ（`#process`）
7. RESULTS — 実績・サポートアカウント（`#results`）
8. MESSAGE FROM GM
9. ROADMAP
10. VOICE — お客様の声
11. PRICING — 料金（`#pricing`）
12. WHY US — パートナーとして
13. FAQ（`#faq`）
14. 流れる帯
15. CONTACT — 最終CTA（`#cta`）
16. フッター
17. 画面下部の固定CTAバー（スマホのみ）

## 6. 画像の差し替え

`images/` 内の同名ファイルを上書きしてください。

- `gm.jpg` — 正方形推奨（円形に切り抜かれます）
- `account-1〜3.jpg` — 正方形推奨（円形に切り抜かれます）

画像が存在しない場合は自動的に非表示になり、レイアウトは崩れません。
