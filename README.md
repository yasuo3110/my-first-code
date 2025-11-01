# my-first-code

GitHub Issues を掲示板ログとして公開するサンプルです。以下のページにアクセスすると、リポジトリ `yasuo3110/my-first-code` の Issue がモバイル対応のレイアウトで表示されます。

- 公開 URL: https://yasuo3110.github.io/my-first-code/

## 使い方

1. 上記 URL をブラウザで開き、掲示板ログとして最新の Issue を確認します。
2. 投稿したい場合は、ページ内の「新規投稿（GitHub Issue）」ボタン、または直接 [Issue 作成画面](https://github.com/yasuo3110/my-first-code/issues/new) を開き、タイトルと本文を入力してください。
3. コメントを追加したい場合は、掲示板の各カードにあるリンクから GitHub 上の対象 Issue に移動してコメントを投稿します。

## Google Sites への埋め込み

Google Sites に表示したい場合は、`埋め込み > 埋め込みコード` を選び、以下のように iframe を追加してください。

```html
<iframe
  src="https://yasuo3110.github.io/my-first-code/"
  width="100%"
  height="600"
  frameborder="0"
  allowfullscreen
></iframe>
```

## 技術メモ

- ページは GitHub Pages でホストされている静的 HTML（`index.html`）です。
- GitHub REST API を利用して最新の Issue を取得し、最大 50 件まで表示します。
- Pull Request は一覧から除外し、本文はプレーンテキストをサニタイズして改行を保持したまま表示しています。
