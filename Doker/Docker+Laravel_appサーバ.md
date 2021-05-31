# アプリケーションサーバ(app)コンテナを作る
## ディレクトリ構成
```
.
├── infra
│   └── php
│       ├── Dockerfile
│       └── php.ini # PHPの設定ファイル
├── backend # Laravelをインストールするディレクトリ
└── docker-compose.yml
```
## docker-compose.ymlを作成
docker-compose.yml
```
version: "3.8"
services:
  app:#=>サービス名:任意で決められる
    build: ./infra/php
    volumes:
      - ./backend:/work
```

- version: DockerComposeファイルのバージョン
  - 通常メジャー、マイナーバージョン両方指定する

- build: `docker build`を実行する際の作業ディレクトリ(**ビルドコンテキスト**)をしていする。
  - DockerFileの存在するディレクトリを指定する。

- volumes: ホスト側のディレクトリや名前付きボリュームをコンテナ側へマウントしたい時に指定する。

## Dockerfileを作る
`FROM php:8.0-fpm-buster`

イメージを作るためのベースイメージ(FROM イメージ名:タグ名)

## php.iniを作成する。
php.ini: PHPの設定ファイル
