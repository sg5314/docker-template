# template-flask
flaskの環境構築のためのDocker環境テンプレート

***

> **Note**
> ### はじめに "必ず" すること
> requirements.txtに必要なPythonパッケージ（+バージョン）を指定

***

### 環境構築＆環境内に入る
1. ビルド　`docker-compose build`
1. コンテナを構築、起動`docker-compose up -d`
1. 起動したコンテナに入る`docker exec -it flask bash`

***

### サーバーの起動
```bash
python app.py
```
これでアクセス可能に http://localhost:3000

