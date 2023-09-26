# make_eigopark_containers

エイゴホイクパークの環境構築用
1. リポジトリをgit cloneしてローカルに落とす
2. _docker-compose.ymlをコピーし、docker-compose.ymlファイルを作成
3. ymlファイルのDB情報をエイゴパークに合わせ、docker-compose up -dでコンテナを起動する
4. エイゴパークのソースファイルをwpコンテナへマージする
5. localhost:8080からwordpressの初期設定をし、ログイン、プラグインをエイゴパークに合わせて有効化する（※All In One WP Securityは除く）
6. localhost:8888からphpMyAdminへログインして、エイゴパークのDBをインポートする
7. localhost:8080/wp-adminからダッシュボードへ入り、設定 >> パーマリンクから「更新を保存」をクリックする
