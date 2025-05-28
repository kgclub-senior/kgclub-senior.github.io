# 関学クラブシニア公式サイト
_Jekyll × Tailwind CSS × Alpine.js スターター_

このリポジトリは **関学クラブシニア** の公式サイトを管理するためのソースです。
Jekyll を土台に、Tailwind CSS と Alpine.js を統合したモダンな静的サイト構成になっています。
ローカルでのプレビューや記事投稿、スタイル調整手順を以下にまとめました。

---

## ✅ クイックスタート

### 1. リポジトリをクローン

```bash
git clone https://github.com/kgclub-senior/kgclub-senior.github.io.git
cd kgclub-senior.github.io
```

### 2. Ruby 依存をインストール

```bash
bundle install
```

### 3. Node.js 依存をインストール

```bash
npm install
```

### 4. Tailwind をウォッチ（別ターミナル推奨）

```bash
npx tailwindcss -i ./assets/css/main.css -o ./assets/css/output.css --watch
```

### 5. Jekyll サーバーでプレビュー

```bash
bundle exec jekyll serve
```

ブラウザで `http://localhost:4000` にアクセスして確認してください。

---

## ✍️ 執筆者向けガイド　操作例

| やりたいこと | 方法 |
|--------------|------|
| 記事を書く | `_posts/YYYY-MM-DD-title.md` を追加し Markdown で本文を書く |
| 画像を置く | `assets/img/` に配置し、記事から相対パスで参照 |
| スタイル調整 | Tailwind クラスを直接 HTML / Markdown 内に記述 |
| コンポーネント化 | `_includes/` 下にパーシャルを作成し、`{% include %}` で呼び出し |

> **ポイント**
> - Markdown の Front Matter（冒頭の `---` ブロック）に `title`, `author`, `categories` などを記述
> - 記事を追加したら **Pull Request** を作成してレビューを受けてください

---

## 🔧 技術スタック

- **Jekyll 4.x** – 生成エンジン
- **Tailwind CSS** – ユーティリティファーストな CSS フレームワーク
- **Alpine.js** – 軽量なインタラクティブ JS ライブラリ
- **PostCSS** – Tailwind のビルド & autoprefixer
- **jekyll-postcss-v2** – Jekyll で PostCSS を動かすプラグイン

---

## 📐 ディレクトリ構成のポイント

```
.
├─ _posts/              # 記事 (Markdown)
├─ _layouts/            # レイアウトテンプレート
├─ _includes/           # 部品テンプレート
├─ assets/
│   ├─ css/
│   │   ├─ main.css     # Tailwind ディレクティブ
│   │   └─ output.css   # ビルド結果 (自動生成)
│   └─ img/             # 画像
└─ _config.yml          # Jekyll 設定
```

---

## 📜 ライセンス

Copyright © 関学クラブシニア
