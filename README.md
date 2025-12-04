# Toshio Iwai Archive

岩井俊雄氏のアーカイブウェブサイト。

作品、展覧会、メディア掲載などの情報を公開しています。

## リポジトリ構成

```
opendata/
└── website/           # Hugo 静的サイト
    ├── content/       # サイトコンテンツ
    ├── themes/        # Hugo テーマ
    └── hugo.toml      # Hugo 設定
```

## ウェブサイト開発

詳細は `website/readme.md` を参照してください。

### ローカル開発

```bash
cd website
hugo server -D
```

ブラウザで http://localhost:1313/ を開いてプレビューできます。

### 本番ビルド

```bash
cd website
hugo
```

ビルド成果物は `website/public/` に出力されます。

## デプロイ

GitHub Actions により自動的にビルド・デプロイされます。

- **公開URL**: https://toshioiwai-archive.github.io/

## 技術スタック

- **静的サイトジェネレーター**: Hugo v0.145.0+
- **ホスティング**: GitHub Pages
- **CI/CD**: GitHub Actions
