<div id="top"></div>

## 使用技術一覧

<!-- シールド一覧 -->
<!-- 該当するプロジェクトの中から任意のものを選ぶ-->
<p style="display: inline">
  <!-- フロントエンドのフレームワーク一覧 -->
  <img src="https://img.shields.io/badge/-Next.js-000000.svg?logo=next.js&style=for-the-badge">
  <img src="https://img.shields.io/badge/-React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB">
  <!-- バックエンドのフレームワーク一覧 -->
  <img src="https://img.shields.io/badge/-Rails-CC0000.svg?logo=rails&style=for-the-badge">
  <!-- バックエンドの言語一覧 -->
  <img src="https://img.shields.io/badge/-Ruby-CC342D.svg?logo=ruby&style=for-the-badge">
</p>

## 目次

1. [プロジェクトについて](#プロジェクトについて)
2. [環境](#環境)
3. [ディレクトリ構成](#ディレクトリ構成)
4. [開発環境構築](#開発環境構築)

<br />
<!-- プロジェクト名を記載 -->

## プロジェクト名

ToDoアプリ

<!-- プロジェクトについて -->

## プロジェクトについて

CRUDを使用したToDoアプリの作成


## 環境

<!-- 言語、フレームワーク、ミドルウェア、インフラの一覧とバージョンを記載 -->

| 言語・フレームワーク  | バージョン |
| --------------------- | ---------- |
| React                 | 18.2.0     |
| Next.js               | 14.0.4     |
| Ruby                  | 3.1.4      |
| Rails                 | 7.0.8      |

その他のパッケージのバージョンは pyproject.toml と package.json を参照してください


## ディレクトリ構成

<!-- Treeコマンドを使ってディレクトリ構成を記載 -->

❯ tree -a -I "node_modules|.next|.git|.pytest_cache|static" -L 2
.
├── .devcontainer
│   └── devcontainer.json
├── .env
├── .github
│   ├── action
│   ├── release-drafter.yml
│   └── workflows
├── .gitignore
├── Makefile
├── README.md
├── backend
│   ├── .vscode
│   ├── application
│   ├── docs
│   ├── manage.py
│   ├── output
│   ├── poetry.lock
│   ├── project
│   └── pyproject.toml
├── containers
│   ├── django
│   ├── front
│   ├── mysql
│   └── nginx
├── docker-compose.yml
├── frontend
│   ├── .gitignore
│   ├── README.md
│   ├── __test__
│   ├── components
│   ├── features
│   ├── next-env.d.ts
│   ├── package-lock.json
│   ├── package.json
│   ├── pages
│   ├── postcss.config.js
│   ├── public
│   ├── styles
│   ├── tailwind.config.js
│   └── tsconfig.json
└── infra
    ├── .gitignore
    ├── docker-compose.yml
    ├── main.tf
    ├── network.tf
    └── variables.tf


## 開発環境構築

<!-- コンテナの作成方法、パッケージのインストール方法など、開発環境構築に必要な情報を記載 -->

### フロントエンドサーバの起動

フロントエンドのディレクトリ配下でコマンドを入力し、サーバを起動させる<br/>
コマンド: npm run dev

### 動作確認

http://localhost:3001 にアクセスできるか確認<br/>
アクセスできたら成功

### サーバの停止

以下のショートカットでサーバを停止することができます

 MacBook: control + C<br/>
 Windows: ctrl + Q

### バックエンドサーバの起動

バックエンドのディレクトリ配下でコマンドを入力し、サーバを起動させる<br/>
コマンド: bundle exec rails s

### 動作確認

http://localhost:3000 にアクセスできるか確認<br/>
アクセスできたら成功

### サーバの停止

以下のショートカットでサーバを停止することができます

 MacBook: control + C<br/>
 Windows: ctrl + Q

### コマンド一覧

| Make                | 実行する処理                                                            |                                                                                |
| ------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| npm run dev         | フロントエンドサーバの起動 |                  |
| bundle exec rails s | バックエンドサーバの起動                                                          |                                                                        |


