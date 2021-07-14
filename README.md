# sample-ajax
授業中のリソースの置き場所

ajaxのgetを行う為のテンプレート
## jQuery側のjsonオブジェクトの準備
```javascript
formData = {};
```
{}は空のjsonオブジェクト
```javascript
formData["param1"] = "テスト";
```
formDataのプロパティはformDat["プロパティ文字列"]に値をセットして作成される

formDataのプロパティはformDat.プロパティ文字列と書くこともできます
```javascript
formData.param1 = "テスト";
```
## jQuery側からサーバへデータを送る
```javascript
data: formData
```
