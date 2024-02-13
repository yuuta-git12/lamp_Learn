Linuxのバージョン：
Apacheのバージョン：2.4.58
MySQLのバージョン：8.0.36
PHPのバージョン：8.3

# 説明
- PHP学習用のリポジトリ

## 参考
- 開発環境構築の参考サイト
  - 開発環境はほぼこれを参考に作成
    - https://qiita.com/are-38-a/items/fbd08334a7d613c3d824
  - [Docker で Apache + PHP コンテナを作る方法](https://lazesoftware.com/ja/blog/230220/)
  - [DockerでApache+PHP+MySQLの環境を構築してみる](https://qiita.com/me-654393/items/1ed212cb33eafe734835)
  - https://zenn.dev/ikuraikura/articles/d166724f2c123d1db312
  - https://zenn.dev/dragonarrow/articles/b3fbdf1718a812
- Apacheの参考サイト
  - [a2enmodとa2dismodコマンドの動作について](https://web.just4fun.biz/?Apache/a2enmodとa2dismodコマンドの動作について)
  - [mod_rewriteとは](https://qiita.com/miyuki_samitani/items/b22e1738b2737c655785)
  - [Apache deflate,exporesについて](https://serverlog.jp/apache2-2/)


## MySQL
https://www.javadrive.jp/mysql/user/index9.html
https://qiita.com/RayDoe/items/baf53818ec8e44d4d148


# メモ
- docker-compose.ymlやDockerfileを含むプロジェクトのディレクトリでは大文字は使えない
- docker実行時にエラーとなる
- docker-composeに書くservices：以下の内容も小文字で書くこと
- 過去に作ったdockerコンテナ PHP_STUDYを再度確認して、内容をリファクタリングする

## 学習用の開発環境
- 以下の環境をDockerで構築
  - サーバー：Apache 最新バージョン
  - プログラミング言語：PHP　バージョン8以降
    - インストールする拡張モジュール
      - OPcache(https://www.php.net/manual/ja/intro.opcache.php)
      - intl(https://www.php.net/manual/ja/book.intl.php)
      - GD(https://www.php.net/manual/ja/book.image.php)
      - Exif(https://www.php.net/manual/ja/book.exif.php)
      - Imagick(https://www.php.net/manual/ja/book.imagick.php)
      - mysqli(https://www.php.net/manual/ja/book.mysqli.php)
      - pdo_mysql(https://www.php.net/manual/ja/book.pdo.php)
      - redis()
      - xdebug(https://xdebug.org)
  - データーベース：postgresql
  - 
## 拡張機能
- Emmmet:入力の効率化用プラグイン html:5でhtmlのページの外枠が一気に入力できる