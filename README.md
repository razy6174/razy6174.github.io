# 昆野 和也のポートフォリオサイト

このリポジトリは、**昆野 和也（Kazuya Konno／GitHub: [razy6174](https://github.com/razy6174)）のポートフォリオサイト**のソースコードです。

公開URL: **https://razy6174.github.io/**

金沢工業大学 情報理工学部 情報工学科に在籍し、情報セキュリティを軸に開発をしています。サイトでは、これまでの制作物・課外活動・受賞歴・スキルを紹介しています。

## 構成

フレームワークやビルドを使わない静的サイトです。`main` ブランチのルートを GitHub Pages で公開しています。

| ファイル | 内容 |
|---|---|
| `index.html` | ページ本体（内容はすべてここに書いています） |
| `styles.css` | スタイル（ライト／ダークの両方に対応） |
| `favicon.svg` | ファビコン |

## アイコン

アイコンには [Lucide](https://lucide.dev)（ISC License）を使っています。使うアイコンの SVG を `index.html` 冒頭の `<svg style="display:none">` 内に `<symbol id="i-アイコン名">` として埋め込み、本文からは次のように参照しています。

```html
<svg class="icon" aria-hidden="true"><use href="#i-shield"/></svg>
```

新しいアイコンを使うときは、lucide.dev から SVG の中身（`<path>` など）をコピーし、同じ形式の `<symbol>` を追加してください。

## ローカルでの確認

`index.html` をブラウザで開くか、次のコマンドで簡易サーバーを立てて http://localhost:8080 を開きます。

```bash
python -m http.server 8080
```
