# Zenn GitHub連携用テンプレートリポジトリ

## テンプレートの使用

[テンプレートからリポジトリを作成する](https://docs.github.com/ja/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)

## VSCode設定

[.vscode/settings.json](./.vscode/settings.json) の設定はお好みで

## Docker

[docker-compose.yml](./docker-compose.yml)があるディレクトリで  
下記のコマンドを実行する。

```sh
docker-compose up
```

## Zenn CLI

### プレビュー

[.env](./.env) ファイルがデフォルト設定であれば  
下記のURLで確認ができる。

- <http://127.0.0.1:8000/>

### コマンド

本環境では、下記のコマンドで実行する。

```sh
docker exec -it zenn-cli [Zenn CLIコマンド]
```

### 記事の作成

```sh
# npx zenn new:article
docker exec -it zenn-cli npx zenn new:article
# slugを指定して追加する場合
docker exec -it zenn-cli npx zenn new:article --slug "slug値"
```

### 本の作成

```sh
# npx zenn new:book
docker exec -it zenn-cli npx zenn new:book
# slugを指定して追加する場合
docker exec -it zenn-cli npx zenn new:book --slug "slug値"
```

## 投稿記事の削除

ダッシュボードからしか行えない。

- <https://zenn.dev/dashboard>

## 参考

### Zenn公式

- [Zenn公式](https://zenn.dev/zenn)
- [GitHub](https://github.com/zenn-dev/zenn-docs)
- [投稿カテゴリー「Tech」「Idea」の選び方](https://zenn.dev/tech-or-idea)
- [Zenn CLIで記事・本を管理する方法](https://zenn.dev/zenn/articles/zenn-cli-guide)
- [GitHubリポジトリ連携で画像をアップロードする方法](https://zenn.dev/zenn/articles/deploy-github-images)
- [ZennのMarkdown記法一覧](https://zenn.dev/zenn/articles/markdown-guide)

### その他

- [node - Official Image](https://hub.docker.com/_/node)
