# Practical Docker Deploy

FastAPI (Backend) + Next.js (Frontend) + MySQL を Docker で構築・デプロイするための実践的サンプルプロジェクトです。
Azure App Service と GitHub Actions を使用した CI/CD パイプラインの構築デモとして使用できます。

## 🚀 技術スタック

* **Frontend**: Next.js 15 (App Router)
* **Backend**: Python 3.12 (FastAPI)
* **Database**: MySQL 8.0
* **Infrastructure**: Docker, Docker Compose
* **Cloud / CI/CD**: Azure App Service, Azure Container Registry, GitHub Actions

## 🛠️ ローカル環境での起動方法 (Docker)

Docker Desktop がインストールされている環境であれば、コマンド一つで環境構築が完了します。

### 1. リポジトリのクローン

```bash
git clone https://github.com/aripoyo14/practical_docker_deploy.git
cd practical_docker_deploy

```

### 2. 環境変数の設定（任意）

`docker-compose.yml` 内でデフォルト値が設定されていますが、必要に応じて `.env` ファイルを作成してください。

### 3. コンテナの起動

```bash
docker-compose up --build

```

初回はイメージのビルドと依存関係のインストールが走るため、数分かかります。

### 4. 動作確認

起動後、以下のURLでアクセスできます。

* **Frontend**: http://localhost:3000
* **Backend API Docs**: http://localhost:8000/docs
* Swagger UI から API のテストが可能です。



## 📂 ディレクトリ構造

```text
.
├── backend/            # FastAPI アプリケーション
├── frontend/           # Next.js アプリケーション
├── .github/workflows/  # GitHub Actions 設定ファイル
└── docker-compose.yml  # ローカル開発用 Docker 構成

```

## 📖 解説記事

本リポジトリの構築手順やデプロイ方法の詳細は、以下の記事を参照してください。

* [Qiita記事へのリンクなどがあればここに貼る]
