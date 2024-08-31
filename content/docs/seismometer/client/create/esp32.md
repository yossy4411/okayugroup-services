+++
title = 'Esp32'
date = 2024-08-31T07:36:48+09:00
draft = true
+++

# ESP32で震度計を作ろう！

## 必要なもの

Wi-Fi（別途通信料が発生する場合があります）

はんだ

以下が購入が必要なものです。全て秋月電気通商で購入が可能です。

| 名前+リンク                                                                    | 価格 ※2024/8現在 | 個数 |
|---------------------------------------------------------------------------|--------------|----|
| [Seeed Studio XIAO ESP32C3](https://akizukidenshi.com/catalog/g/g117454/) | 1080円        | 1個 |
| [KXR94-2050](https://akizukidenshi.com/catalog/g/g105153/)                | 850円         | 1個 |
| [ユニバーサル基板](https://akizukidenshi.com/catalog/g/g103229/)                  | 60円          | 1枚 |
| [コンデンサ(3300pF)](https://akizukidenshi.com/catalog/g/g108120/)             | 120円         | 3個 |

### それぞれの役割

- Seeed Studio XIAO ESP32C3: マイコン
- KXR94-2050: 加速度センサー
- ユニバーサル基板: 配線用
- コンデンサ(3300pF): ノイズ対策

## 作成手順

1. Seeed Studio XIAO ESP32C3にKXR94-2050を接続します。
2. ユニバーサル基板にコンデンサを接続します。
3. Seeed Studio XIAO ESP32C3にプログラムを書き込みます。
4. トークンを取得します。
5. プログラムを実行し、設定を行います。
6. データをサーバーに送信します。
7. Viewerでデータを確認します。

## プログラム

[GitHub](https://github.com/yossy4411/seismometer-esp32)よりダウンロードしてください。（作成中）
