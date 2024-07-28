+++
title = 'GUIが使えない環境での編集'
date = 2024-07-28T18:28:13+09:00
draft = false
+++

もしGUIが使えない環境、またはファイルを`--nogui`引数付きで起動している場合、`inputs.json`ファイルを編集してイベントを編集できます。

`inputs.json`のフォーマットは以下の通りです。

## 構文

```js
{
    "events": [
        // イベントを格納する
        {
            "links" : [
                1 
                // このノードが接続している別のノードの、events内でのインデックス
             ],
            "event" : {
            "type" : "", //イベントの名前
            "args" : [
                ""
                // イベントの引数
             ]
            },
            "x" : 0, // 画面内でのX座標
            "y" : 0, // 画面内でのY座標
            "width" : 200.0, // 画面内での横幅
            "height" : 200.0, // 画面内での縦幅
            "async" : false // 非同期処理を使用するか
        }
    ],
    "input": {
        // Webでの入力イベントを定義する
        "parent" /*Web上の親名*/ : {
            "child" /*Web上での子名*/ : 0 /*インデックス*/
        }
    }
}
```

## サンプル


```js
{
    "events" : [ 
        {
            "links" : [ 1 ],
            "event" : {
            "type" : "RequestEvent",
            "args" : [ "run1", "test" ]
            },
            "x" : 50,
            "y" : 100,
            "width" : 200.0,
            "height" : 100.0,
            "async" : false
        }, {
            "links" : [ ],
            "event" : {
                "type" : "ConsoleCommand",
                "args" : [ "ls" ]
            },
            "x" : 300.0,
            "y" : 100.0,
            "width" : 200.0,
            "height" : 100.0,
            "async" : false
        }
    ],
    "input" : {
        "test" : {
            "run1" : 0
        }
    }
}
```

`input.json`を作成し、上記をコピー・ペーストします。

**アプリを再起動してから**`http://<IPアドレス>:8080/test/run1`にアクセスすると実行が可能です。

