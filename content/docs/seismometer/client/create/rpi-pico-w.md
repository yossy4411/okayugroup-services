+++
title = 'Raspberry Pi Picoで震度計を作ろう！'
date = 2024-06-22T16:02:14+09:00
draft = false
+++

## 注意事項

**非推奨です**

Raspberry Pi Picoは、ESP32などのマイコンに比べて性能が低く、少し高価なため、非推奨としております。
また、 ADXL367はノイズがひどく、これらのものでは正確な地震計を作成できないと判断しました。

より正確な地震計を作成するためには、[ESP32](/docs/seismometer/client/create/esp32)を使用してください。

ソフトウェアは開発ストップ状態で、今後も更新する予定はありません。

## 必要なもの

Wi-Fi（別途通信料が発生する場合があります）

はんだ

以下が購入が必要なものです。全て秋月電気通商で購入が可能です。

| 名前+リンク                                                                  | 価格    | 個数   | 
|-------------------------------------------------------------------------|-------|------|
| [Raspberry Pi Pico W セット](https://akizukidenshi.com/catalog/g/g118021/) | 1340円 | 1個   |
| [AE-ADXL367](https://akizukidenshi.com/catalog/g/g129428/)              | 1240円 | 1個   |
| [ブレッドボード](https://akizukidenshi.com/catalog/g/g105294/)                 | 220円  | 1枚   |
| [ジャンパーワイヤ(18本以上入)](https://akizukidenshi.com/catalog/g/g105371/)        | 180円  | 6本   |
| 送料                                                                      | 500円  | 購入ごと |
| 合計                                                                      | 3480円 |      |


## 作成手順

1. Raspberry Pi Pico WにAE-ADXL367を接続します。
2. ブレッドボードにAE-ADXL367を接続します。
3. Raspberry Pi Pico Wにプログラムを書き込みます。
4. プログラムを実行します。
5. データをサーバーに送信します。

## プログラム

[GitHub](https://github.com/yossy4411/seismometer-rpi-picow)よりダウンロードしてください。（作成中）

## ライセンス

GPL-3.0 License &copy; 2024 [OkayuGroup (おかゆグループ)](https://okayugroup.com)