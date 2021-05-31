# Dockerfile
世界一わかりみが深いコンテナ & Docker入門 〜 その3:Dockerfileってなに？ 〜[https://tech-lab.sios.jp/archives/19191](url)

Dockerのイメージを作成するコマンドを一つのファイルにまとめたもの。

## 話の流れ
- コンテナ　→　仮想OSがなくても環境がつくれる。
- コンテナを作るにはもろもろの作業が必要　→　Dokerのコマンドで全部やってくれる
- 目的のコンテナを作るためのレシピ　→　Dockerfile
- 各コンテナの設定 -> docker-compose.yml(ここに呼び出すDockerfileを記す。)