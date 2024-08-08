+++
title = 'IoT-Home'
date = 2024-07-27T13:40:07+09:00
draft = false
+++

# IoT-Homeアプリ

## 概要

IoT-Homeは、インターネット上のRestfulAPIを通じてPC上でリモートにイベントを実行するためのアプリケーションです。

家庭・社内でのIoT向けに作成されました。

### 対応機種

Javaが使用可能なすべてのデバイス。以下に例を示します。
 - Windows
 - MacOS
 - Linux (Ubuntu, Debian, CentOS...)

## 使い方
ノードを接続するだけでイベントを作成できます。 詳細: [ノード接続の基本](/docs/iot-home/connect)

## インストール

1. GitHubから[最新版](https://github.com/yossy4411/IoT-Home/releases/latest)のiot-home.zipをダウンロードしてください。
2. ダウンロードしたzipファイルを解凍し、任意の場所に配置します。
3. 解凍したディレクトリに移動し、iot-home.jarファイルをダブルクリックするか、以下のコマンドを使用して起動します。
   ```bash
   java -jar iot-home.jar
   ```
4. GUIが起動します。GUIが起動できない環境の場合は[こちら](/docs/iot-home/console)のドキュメントをご覧ください。

## ライセンス

GNU General Public License 3.0

[LICENSE (GitHub)](https://github.com/yossy4411/IoT-Home/blob/master/LICENSE)
