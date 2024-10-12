# docker-react-typescript
※こちらは最新のtypescript版です。

旧:js版は[こちら](https://github.com/Kartis0207/docker-react)


react の docker プロジェクト

参考：https://github.com/StephenGrider/docker-react

### docker

#### docker で当プロジェクトをビルド

```bash
docker-compose build
```

#### docker で当プロジェクトを起動

```bash
docker-compose up -d
```

これで接続できる

### 動作確認

#### react

http://localhost:3000/

### メモ
vscode等で開発する場合、node_modulesの関係でvscode上の依存関係が解決できません。
これは、docker上のnode_modulesをローカルがマウントしないため発生しています。
本アプリにおいては、本番環境へのデプロイを考慮し、デフォルトではローカル環境のnode_modulesへのマウントはしない設定となります。
アプリの動作には影響ないですが、vscode上のエラーが気になる場合は
別途　ローカルにて npm install を行うと発生しなくなります。


参考：https://github.com/StephenGrider/docker-react
