# Research notes

森本尊礼の研究ブログ。Quarto + GitHub Pages。日本語 `/ja/`、英語 `/en/`。
Quarto公式 `quarto create project blog` のテンプレート（Cosmo、標準記事一覧、Jollaプロフィール）を使用。

## ローカル確認

Quarto 1.10.19をインストールし、このディレクトリで `quarto preview`。
`quarto render` で `_site/` に出力する。

## 記事を書く

1. ローカルの `_drafts/` で原稿を用意する。このフォルダはGit管理・公開の対象外。
2. 問い、仮説、実験条件、結果、解釈、限界、再現方法を記述する。
3. 公開承認後、日本語を `ja/posts/<slug>/index.qmd`、英語を `en/posts/<slug>/index.qmd` に置く。
4. 記事の先頭にYAMLで `title`、`date`、`description`、`categories`、`lang` を指定する。記事一覧へは自動で追加される。対応記事同士もリンクする。
5. `quarto render` と画面確認後、mainへpushするとGitHub Actionsが公開する。

公開リポジトリのため、**下書き・非公開実験・秘密情報はコミットしない**。
`draft: true` はソースの秘匿手段ではない。

英訳は執筆時に作成し、数値・専門用語・主張の強さを確認する。自動翻訳APIは使用しない。
