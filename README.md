# http-redirect

httpアクセスをリダイレクトするコンテナです。
Dockerで動かしていたWebサービスを移転したとき、新URLに転送するのにどうぞ。

docker-compose.ymlの下記の箇所をお好みで書き換えて、旧サーバに設置してください。

```
ports:
  - "8080:80"
environment:
  - REDIRECT_TO=http://foobar.com/
```
