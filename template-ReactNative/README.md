# template-ReactNative
## React Nativeの環境構築のためのDocker環境テンプレート

<details><summary>初期構築</summary>

1. envファイルが作成される（ipアドレスが記入される）
```bash
make expo_sample
```

2. プロジェクトテンプレートを選択 -> プロジェクトのセットアップが開始
```bash
docker-compose exec react_native bash
expo init .
```
3. スタート
```bash
expo start
```

</details>

---

### 2回目以降
* envファイルは一度削除した方がいい
```bash
make expo_sample
docker-compose exec react_native bash
expo start
```

### Expo（必要なアプリ）

1. Expoアカウントを作成（[Expoアカウントの作成方法](https://qiita.com/hidenoritoki/items/0c5084b84dfc2126d9ec)）

2. Expoクライアントアプリのインストールとセットアップ</br>
（[iPhoneでExpoクライアントアプリのインストールとセットアップ方法](https://qiita.com/hidenoritoki/items/afa69ca6ce910ee28cd9)）

