# 職務経歴書

## 基本情報


|---|---|
|氏名|宮本幸太郎|
|生年月日|1999/07|
|Twitter||
|Qiita||
|note||
|Zenn||


---


## 技術スタック

### 言語

|---|---|
|Python|3年|
|TypeScript|1.5年|


### フレームワーク

|---|---|
|Django|3年|
|Nest.js|0.5年|
|Next.js|1.0年|


### DB

|---|---|
|MySQL|3年|
|PostgreSQL|1.5年|
|MongoDB Atlas|2年|

### インフラ

|---|---|
|AWS|1.5年|
|GCP|1年|
|Docker|1.5年|

### ツール
- Git
- GitHub
- VScode
- Teams
- Jira

---

## 職務経歴詳細

### 大手ソフトウェア会社の社内人事システム開発 (2024 年 4 月〜 現在)

マイクロサービスアーキテクチャで開発されている大手ソフトウェア会社の社内人事システムの開発をフルスタックで担当。

|---|---|
| 担当工程 | 詳細設計 〜 開発 |
| チーム人数 | 2人 |
| 役割 | SE |

- **使用技術**
  - OS
    - Ubuntu
  - 言語
    - TypeScript
  - FW
    - Next.js
    - Nest.js
  - DB
    - MySQL
  - ツール
    - Jira
    - GitLab

- **担当業務詳細**
  - gRPCサーバの構築
  Protocol Bufferで定義したファイルからTypeScriptの型を自動生成するスクリプトを構築。DDD + CQRSで設計されたアーキテクチャのBFFからリクエストされるgRPCサービスを実装。
  - BFFの実装
  gRPCサーバへリクエストするインターフェースを作成。API規格はGraphqlを使用。gRPCのエラー内容をGraphqlのエラーとして扱えるようレスポンス用のクラスを実装。
  - フロントエンドの実装
  Atomic Designでコンポーネントを切り分け、社内のUIライブラリにも作成したコンポーネントを追加。フロント担当のインターン生のタスク管理も担当。


### 本人確認システムを組み込んだ物件申込システムの開発 (2023 年 8 月〜 2024年 4月)

居抜き物件の申込サイトの基本設計以降を担当


|---|---|
| 担当工程 | 基本設計 〜 開発 |
| チーム人数 | 4人 |
| 役割 | PG |

- **使用技術**
  - OS
    - Ubuntu
  - 言語
    - TypeScript
  - FW
    - Next.js
    - React
  - DB
    - MySQL
  - インフラ
    - Google Cloud Run
    - Google Cloud SQL
  - ツール
    - Git
    - GitHub
    - Redmine
    - Azure Devops

- **担当業務詳細**
  - 顧客情報期間システムとの連携バッチ設計・開発
  申込サイトで入力された情報をお客様の期間システムに連携するバッチの設計と開発を担当。Google Cloud FunctionとCloud Schedulerで実装。
  - Azure DevopsからCloud RunへのCI/CD構築
  mainブランチへデプロイした際にAzure Devops => Artifact Registry => Cloud Runへ自動デプロイするCI/CDを構築。
  - 申込サイトでアップロードされたファイルのウイルススキャンサーバーの構築
  ClamAVのイメージからコンテナを生成し、Cloud Runへデプロイ。申込サイトでアップロードされたファイルをClamAVでスキャンし結果を返すサーバを構築。
  - DB登録時のパフォーマンスアップ
  多くのファイルデータを扱うためDB登録時の処理に時間がかかっていたのを一度Cloud Storageに非同期でアップロードしファイルのIDをDBに保存 => データ連携バッチでファイルデータを基幹システムへ連携するという形に変更することで登録処理時間を 7秒 → 0.5秒以内 に短縮。

### 行政が運営するスポーツ施設の予約システムの開発 (2022 年 12 月〜 2023年 7月)
他者が開発していたシステムを請け負い、リファクタリングと追加機能開発の基本設計〜保守・運用を担当。

|---|---|
| 担当工程 | 基本設計 〜 開発 |
| チーム人数 | 2人 |
| 役割 | PG |

- **使用技術**
  - OS
    - Ubuntu
  - 言語
    - TypeScript
    - Python
  - FW
    - Gatsby
    - React
    - Django
  - DB
    - MongoDB
  - インフラ
    - Google Cloud Run
    - Google Cloud SQL
    - Docker
  - ツール
    - Git
    - GitHub
    - Redmine
    - Azure Devops

- **担当業務詳細**
  - 他者が開発したモバイルアプリとの連携
  予約システムが保持しているユーザーアカウント情報で他者が開発しているモバイルアプリでもログイン + ユーザーの権限管理が出来るようAuth0のClient Credentialを使用した連携方法の設計を担当。また外部の担当者との質問対応窓口も担当。
  - 既存コードのテストコードを追加
  請け負った際にテストコードが記載されていなかった為、仕様書と照らし合わせながらpytestで約4000行のテストコードを構築。テストデータ自動生成やfixtureも構築することでテスト環境も整備する。
  - 見積システムとのアクセストークンを使用したAPIの設計・開発
  見積システムから予約システムへユーザーを取得するAPIを設計・開発し実行時にJWTトークンを使用してクライアントの有効性を検証。

### 行政が運営するスポーツ施設の見積システムの開発 (2022 年 9 月〜 2023年 2月)

|---|---|
| 担当工程 | 基本設計 〜 開発 |
| チーム人数 | 5人 |
| 役割 | PG |

- **使用技術**
  - OS
    - Ubuntu
  - 言語
    - TypeScript
    - Python
  - FW
    - Gatsby
    - React
    - Django
  - DB
    - MongoDB
  - インフラ
    - Google Cloud Run
    - Google Cloud SQL
    - Docker
  - ツール
    - Git
    - GitHub
    - Redmine
    - Azure Devops

- **担当業務詳細**
  - RestAPIからGraphqlへのリファクタリング
  RestAPIで構築していたのを予約システムと統一するためにGraphqlへリファクタリング。
  - 帳票出力サーバーの構築
  見積書や請求書を出力するためのサーバをCarbone.jsで構築。帳票のサンプル作成とお客様との確認業務も担当。
  - 予約システムとの連携APIの設計・開発

### オンライン動画教育サービスのLMSの開発 (2020 年 8 月〜 2022年 8月)

|---|---|
| 担当工程 | 基本設計 〜 開発 |
| チーム人数 | 5人 |
| 役割 | PG |

- **使用技術**
  - OS
    - Windows
  - 言語
    - Python
  - FW
    - Django
  - DB
    - MySQL
  - ツール
    - Git
    - GitHub

- **担当業務詳細**



### 副業

- 更年期オンライン診療アプリの立ち上げ（2023年 10月 ~ 現在）

|---|---|
| 担当工程 | 企画・要件定義 〜 保守・運用 |
| チーム人数 | 2人 |


- **使用技術**
  - OS
    - Ubuntu
  - 言語
    - Python
    - TypeScript
  - FW
    - Django
    - React
  - DB
    - PostgreSQL
  - インフラ
    - AWS RDS
    - AWS AppRunner
    - AWS S3
  - ツール
    - Git
    - GitHub

- **担当業務詳細**
  - 