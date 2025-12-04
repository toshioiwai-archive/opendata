# Toshio Iwai Archive Website

岩井俊雄氏のアーカイブサイト。

## 技術スタック
- フレームワーク: Hugo (v0.145.0+)
- デプロイ: GitHub Actions
- ホスティング: GitHub Pages
- テーマ: toshioiwai（カスタムテーマ）
- 言語: 日本語（デフォルト）+ 英語対応

## ディレクトリ構造

```
website/
├── archetypes/      # コンテンツテンプレート
├── assets/          # CSS, JS などの処理対象アセット
├── content/         # サイトコンテンツ（Markdown）
├── data/            # データファイル（CSV, JSON等）
├── i18n/            # 多言語対応の翻訳ファイル
├── layouts/         # HTMLテンプレート
├── static/          # 静的ファイル（画像、フォント等）
├── themes/          # テーマディレクトリ
│   └── toshioiwai/  # カスタムテーマ
└── hugo.toml        # Hugo設定ファイル
```

## 開発コマンド

### 開発サーバーの起動

```bash
cd website
hugo server -D
```

開発サーバーは http://localhost:1313/ でアクセス可能。

### 本番ビルド

```bash
cd website
hugo
```

ビルドされたファイルは `public/` ディレクトリに出力されます。

### ドラフトも含めてビルド

```bash
cd website
hugo -D
```

## コンテンツ管理

`content/` ディレクトリ配下に、以下のセクションのコンテンツが Markdown 形式で格納されています：

- `content/works/` - 作品情報
- `content/events/` - 展覧会情報
- `content/media/` - メディア掲載情報

各コンテンツは日本語（.ja.md）と英語（.en.md）のファイルがあります。

## デプロイ

GitHub Actions によって自動デプロイされます。
`main` ブランチへのプッシュ時に自動的にビルド・デプロイが実行されます。
