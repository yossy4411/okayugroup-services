+++
title = 'ノードの接続'
date = 2024-07-28T13:01:44+09:00
draft = false
+++

1. パレット上部から 入力>インターネット>WebRequest ノードを取り出します。

![入力から取り出す](/iot-home/images/inputselector.gif)

2. ノードのサイズはウィンドウのように調節することができます。上部を掴んで動かすこともできます。

![ノードサイズ変更](/iot-home/images/windowsize.gif)

3, ノードの引数はクリックすると入力状態になり、キーボードで入力が可能です。

![ノードへの入力](/iot-home/images/eventinput.gif)

3. Linux/MacOSの場合、中間>コンソール>ConsoleCommand ノードを取り出します。ここでは`ls -l`コマンドを実行します。

![Bashコマンド実行](/iot-home/images/linuxcommand.gif)

4. Windowsの場合、 中間>コンソール>PowershellCommand ノードを取り出します。ここでは`ls`コマンドを実行します。

![Windowsコマンド実行](/iot-home/images/wincommand.gif)

5. ノードは右側の「出力ピン」をドラッグしてつなぐことができます。また、ホバーすることで出力値の型が表示されます。

![ノード接続](/iot-home/images/connect.gif)

6. ノード上部をダブルクリックしてノードを削除できます。自動的に接続も解除されます。

![ノード交換](/iot-home/images/change.gif)

7. Webで`localhost:8080/api/<エンドポイント親名>/<エンドポイント子名>`にアクセスすると、イベントが実行されます。