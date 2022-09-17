# template-react
## reactの環境構築のためのDocker環境テンプレート

### ビルド　
```bash
docker-compose build
```

### 初期構築

<details><summary>Reactプロジェクトの生成</summary>

```bash
docker-compose run --rm node sh -c "npm install -g create-react-app && create-react-app {{アプリ名}}"
```

</details>
</br>

### コンテナ起動 && コンテナ内に入る
1. コンテナを構築、起動 `docker-compose up -d`
1. 起動したコンテナに入る `docker exec -it react bash`

***

### サーバーの起動
```bash
npm start
```
これでアクセス可能に http://localhost:3000 
