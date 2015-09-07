/*
Title: Postgresql
Description: Postgresql
*/

### Postgresqlの初期設定


Databaseをインストールした後の手順

* 権限のあるユーザに変更

> sudo su postgres

* ユーザ(ロール)の作成

> createuser [username]

* データベースの作成

> createdb [database name] --owner=[username] --encodeing=UTF8

* 作成作業を一旦終える

> exit

* 再ログイン

> psql [database name]


* パスワードの設定

> ALTER ROLE [username] ENCRYPTED PASSWORD 'password';
