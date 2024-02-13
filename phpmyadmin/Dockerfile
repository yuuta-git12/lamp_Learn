FROM phpmyadmin/phpmyadmin:latest

#ARGでDockerfileで使用する変数定義ができる　UIDに1000を代入
ARG UID=1000
# RUNでLinuxコマンドを実行
# useraddはユーザーを追加
# -m, --create-home：ホームディレクトリを作成します。
# -u, --uid ${UID}：${UID}をユーザーIDとして指定する
# ユーザー名は「dockeruser」とする
RUN useradd -m -u ${UID} dockeruser

# 以降は実行ユーザーをUID = 1000で実行する
USER ${UID}