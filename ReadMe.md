# このソフトウェアについて #

CreateRemoteRepository201610011955は、GitHubのリモートリポジトリ作成を実行するバッチファイル＆シェルスクリプトである。

# 開発環境 #

* Windows XP Pro SP3 32bit
    * cmd.exe
* msys 2013072300
    * msys.bat(sh.exe)
    * [mingw-get.exe](https://sourceforge.net/projects/mingw/files/Installer/mingw-get-setup.exe/download)
* [cURL](https://curl.haxx.se/download.html#Win32) 7.24.0
    * [SSL証明書](http://curl.haxx.se/ca/cacert.pem)
* [nkf](http://www.vector.co.jp/soft/win95/util/se295331.html) 2.1.1 (2010-08-08)

cURL, nkfは環境変数のPathに追加する。

# 使い方 #

## 1. リポジトリ名にしたいディレクトリを用意する ##

任意のディレクトリの配下に、CallShell.bat、CreateRepository.sh、を配置する。

ディレクトリ名は半角英数字と`.`,`-`,`_`の文字だけにすること。
リモートリポジトリがその文字しか使えないため。

## 2. パラメータ設定 ##

`CreateRepository.sh`ファイルのパラメータを任意に設定する。

* CURL_PEM="C:\Program Files\Git\ssl\certs\cacert.pem"
* GITHUB_USER="YourUsername"
* GITHUB_PASS="YourPassword"
* REPO_DESC="リポジトリの説明です。"
* REPO_HOME="https://www.google.co.jp"

## 3. CallShell.batをダブルクリックする ##

GitHubでリモートリポジトリができていることを確認する。

# ライセンス #

このソフトウェアはCC0ライセンスです。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)
