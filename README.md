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
```javascript
{
      "param1": "テスト"
}
```
http://localhost/app/form-action-json.php?param1=%E3%83%86%E3%82%B9%E3%83%88&_=1626243759099

と言うフォーマットに jQuery に加工されてサーバの PHP が呼び出されます
## PHP でデータを受け取る
QuertyString と呼ばれる ? 以降の文字列が $_GET にセットされて PHP に入る
```
param1=%E3%83%86%E3%82%B9%E3%83%88&_=1626243759099
```
