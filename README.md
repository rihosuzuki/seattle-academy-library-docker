# seattle-academy-library-docker

## 手順
1. クローンする
    ```
    git clone git@github.com:ryuya-matsunawa/seattle-academy-library-docker.git
    ```
1. dockerコンテナを起動する
    ```
    docker compose up -d
    ```
1. コンテナが立っているか確認
    ```
    docker ps
    ```
    以下のように3つのコンテナが起動中ならOK

    |  CONTAINER ID  |  IMAGE  |  COMMAND  |  CREATED  |  STATUS  |  PORTS  |  NAMES  |
    | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
    |  4744ee988489  |  postgres:latest  |  "docker-entrypoint.s…"  |  36 minutes ago  |  Up 40 seconds  |  0.0.0.0:5433->5432/tcp  |  seattle_academy_postgres  |
    |  35f5beff2fe9  |  minio/minio:latest  |  "sh -c ' mkdir -p /d…"  |  3 days ago  |  Up 3 days  |  0.0.0.0:9000-9001->9000-9001/tcp  |  seattle_academy_minio  |


### 参考サイト
[Docker で作る postgres 環境](https://crudzoo.com/blog/docker-postgres)