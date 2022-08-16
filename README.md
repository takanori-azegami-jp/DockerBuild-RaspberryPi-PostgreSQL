# DockerBuild-RaspberryPi-PostgreSQL
RaspberryPi(64bit)にDockerでPostgreSQLサーバを構築

## 環境
- kernel：Linux ホスト名 5.15.32-v8+ #1538 SMP PREEMPT Thu Mar 31 19:40:39 BST 2022 aarch64 GNU/Linux
- OS：Debian GNU/Linux 11 (bullseye)

## Dockerコマンド
```bash
# Docker-compose実行
$ docker-compose up -d

# Docker コンテナ確認
$ docker ps

# Docker イメージ確認
$ docker images

# Docker コンテナの中に入る
$ docker exec -it [コンテナID] bash

# dokcer-composeのリビルド
$ docker-compose up -d --build  --force-recreate

# dokcer-composeの一括削除（滅びの呪文）
$ docker-compose down --rmi all --volumes --remove-orphans
```

## 参考サイト
- [【Docker】postgresqlの構築](https://zenn.dev/re24_1986/articles/b76c3fd8f76aec)
- [postgresイメージは使わずにDockerでPostgreSQLに初期データを投入](https://hiroki-sawano.hatenablog.com/entry/populate-postgres-container)
