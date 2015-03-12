# dollarone
エイプリルフールのネタで作った物をここに捨てておく。URLは動作例

[ライセンス](LICENSE.md)

```html
<div class="form-group">
  <label class="col-sm-3 control-label">年齢</label>
  <div class="col-sm-3" ng-class="{'has-success':form.age.$valid && form.age.$dirty,'has-error':form.age.$invalid && form.age.$dirty}">
    <input type="number" class="form-control" name="age" ng-model="age" min="15" max="150" integer required>
    <span class="text-danger" ng-show="form.age.$error.integer">整数値を半角で入力してください</span>
    <span class="text-danger" ng-show="form.age.$error.required && !form.age.$error.integer">必須項目です</span>
    <span class="text-danger" ng-show="form.age.$error.min || form.age.$error.max">範囲外の数値です</span>
  </div>
</div>
```
