# jekyll_tailwind_alpinejs_basic

このプロジェクトは、Jekyll に Tailwind CSS と Alpine.js を統合した基本的なスターターキットです。

## ✅ セットアップ手順

以下の手順に従って、ローカル環境でこのプロジェクトを立ち上げることができます。

### 1. リポジトリのクローン

```bash
git clone https://github.com/your-username/jekyll_tailwind_alpinejs_basic.git
cd jekyll_tailwind_alpinejs_basic
```

### 2. Ruby の依存関係をインストール

```bash
bundle install
```

### 3. Node.js の依存関係をインストール

```bash
npm install
```

### 4. Tailwind のウォッチャーを起動（別ターミナル推奨）

```bash
npx tailwindcss -i ./assets/css/main.css -o ./assets/css/output.css --watch
```

### 5. Jekyll サーバーを起動

```bash
bundle exec jekyll serve
```

その後、ブラウザで `http://localhost:4000` にアクセスしてください。

---

## 🔧 使用技術

- Jekyll 4.x
- Tailwind CSS
- Alpine.js（npm経由またはCDN）
- PostCSS
- jekyll-postcss-v2 プラグイン

---

## 📁 構成のポイント

- `assets/css/main.css` に Tailwind のディレクティブを記述
- `output.css` がビルドされ、`_layouts/default.html` などで読み込まれる
- Tailwind クラスは `npx tailwindcss` のビルドで反映
- `Alpine.js` は `<script>` タグ or npm 経由で読み込み

---

経緯としては、TailwindやAlpine.jsをつかってサイトを作りたい。からJekyllでそれが可能内容最低限の設定をしました。
SCSSではなくCSSで実現し、もともとのデフォルトの設定そのままですがあえてデフォルトには手を加えずにそのまま使えるようにしたものです。
ご自身で0から適用されたい場合は、`jekyll new プロジェクト名 --blank` から始めて、Gemfile・_config.yml・PostCSS・Tailwind の設定などを順に整えていくことで、カスタムテーマ構築にも応用可能です。

## 📄 ライセンス

MIT
