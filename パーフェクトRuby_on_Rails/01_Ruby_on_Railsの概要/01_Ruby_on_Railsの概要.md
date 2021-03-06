# bundlerのコマンド
- bundle initとは
Gemfileを作成する。
- bundle execとは
Bundlerでインストールされているgemパッケージを使用してコマンドを実行する。

# よく利用するrailsコマンド
| コマンド       | 概要                                                                         |
| -------------- | ---------------------------------------------------------------------------- |
| generate (g)   | テンプレーて機能を使ってプログラムの雛形などを生成する                       |
| console (c)    | Railsアプリケーションの環境を読み込んだ上でirbを起動する                     |
| server (s)     | 開発用アプリケーションサーバを起動する                                       |
| test (t)       | アプリケーションのテストを実行する                                           |
| test:system    | アプリケーションのシステムテストを実行する                                   |
| new            | Railsアプリケーションを作成する                                              |
| dbconsole (db) | 設定ファイルに定義されている接続情報を使ってDBへ接続し、コンソールを起動する |
| db:create      | データベースを作成する(SQLite3の場合は不要)                                  |
| db:drop        | データベースを削除する(SQLite3の場合は「.sqlite3」ファイル自体を削除)        |
| db:migrate     | マイグレーションファイルの内容(テーブル定義)をDBに反省させる                 |
| db:seed        | `db/seeds.rb`の内容を実行する                                                |
| db:setup       | データベースを作成し、スキーマの読み込みとシードデータの読み込みを行う       |
| routes         | URLとControllerを紐付けているルーティング情報を出力する                      |
| runner         | 任意のスクリプトを実行する                                                   |
| stats          | ControllerやModelなどの行数などを集計したデータを表示する                    |

# ルーティングの管理とRESTの思想
- ルーティングの確認
1. `rails routes`コマンドによって標準出力で確認
2. ブラウザにて`localhost:3000/rails/info/routes`へアクセスするか存在しないURLを入力して確認
