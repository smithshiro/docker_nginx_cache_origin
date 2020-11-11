# nginx cache origin sample

キャッシュサーバとオリジンサーバをnginxで構成してファイルのキャッシュを確かめる用

## Getting Started

### Prerequisites

docker version
```
$ docker -v
Docker version 19.03.12, build 48a66213fe
```
docker-compose version
```
$ docker-compose -v
docker-compose version 1.26.2, build eefe0d31
```
### Installing

インストール
```
$ docker-compose up -d
```
## Running the tests
キャッシュの場所確認

キャッシュコンテナに入る
```
$ docker-compose exec cache_nginx /bin/bash
```
キャッシュのあるディレクトリ
```
$ cd /var/lib/nginx/cache/
$ ls
nginx nginx_temp
```
