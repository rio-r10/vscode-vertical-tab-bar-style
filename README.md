# 概要

VSCodeでもファイルのタブを縦に並べて表示したい。
IntelliJで縦のタブに慣れていると、VSCodeを使う時に一番ストレスに感じるポイントな気がします。
このCSSを読み込むと、なんとなくそれっぽい雰囲気になります。
<img width="1620" alt="スクリーンショット 2022-01-23 17 14 59" src="https://user-images.githubusercontent.com/37741367/150684327-6668b372-d4bb-41da-8233-f4b8b95d2fd1.png">



# 使い方
1. 任意の場所にCSSファイルを配置する。
2. 下記プラグインでCSSを読み込めるように設定し、1で配置したファイルへのパスをsettings.jsonに追加する。
```
    "vscode_custom_css.imports": [
        "file:///Users/PATH_TO_FILE/vscode-style.css"
    ]
```
3. ファイルのパンくずの表示のstyleは諦めたので、表示をOFFにするようにsettings.jsonに追加する。
```
    "breadcrumbs.enabled": false,
```
3. それっぽくなる。

# 注意
VSCodeのバージョンが違うとclass名が変わったりするので動かない場合があります。
作成時のVSCodeのバージョンは `1.63.2` です。
動かない時は適宜cssを編集して使ってください。
