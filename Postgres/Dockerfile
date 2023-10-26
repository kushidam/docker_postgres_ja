#PostgreSQLイメージをベースに、日本語環境設定を追加
FROM postgres:15.2
#apt-getを更新し、日本語ロケールをインストールして設定
RUN apt-get update && \
    apt-get install -y locales && \
    localedef -i ja_JP -c -f UTF-8 -A /usr/share/locale/locale.alias ja_JP.UTF-8
#LANG環境変数を設定
ENV LANG ja_JP.utf8
#LC_ALL環境変数を設定
ENV LC_ALL ja_JP.utf8
