# template-flutter
flutterの環境構築のためのDocker環境テンプレート

***

> **Note**
> ### はじめに "必ず" すること
> 「env」という名前のファイルを「.env」（ドットをつける）に変更

***

### 環境構築＆環境内に入る
1. ビルド　`docker-compose build`
1. コンテナを構築、起動`docker-compose up -d`
1. 起動したコンテナに入る`docker exec -it flutter bash`

***

### 初期構築
* flutterアプリを作成
```bash
cd ${APP_CODE_PATH_CONTAINER}
flutter create .
```

### サーバーの起動
```bash
flutter run -d web-server --web-port=${WEB_SERVER_PORT} --web-hostname 0.0.0.0
```
これでアクセス可能に http://localhost:8888


<details><summary>Tips</summary>

### Flutterをアップグレードする場合
```bash
flutter upgrade
```

### Webをビルドする場合
```bash
flutter build web
```

### 設定できているか確認したい時
```bash
flutter doctor
```

</details>


* https://github.com/c-a-p-engineer/docker-flutter
