## checkbox

#### 如何控制 checkbox 默认的选择和不选择的值

> 可以使用 ng-true-value 和 ng-false-value 加上 ng-model

```
<input type="checkbox"
       ng-model="string"
       [name="string"]
       [ng-true-value="expression"]
       [ng-false-value="expression"]
       [ng-change="string"]>
```

注意：这里面的 ng-true-value="1" 和 ng-true-value="'1'" 是不一样


#### 扩展阅读：

* [官方 API](https://docs.angularjs.org/api/ng/input/input%5Bcheckbox%5D)
* [官方 DEMO](http://plnkr.co/edit/?p=preview)
* [AngularJS: ng-model not binding to ng-checked for checkboxes](http://stackoverflow.com/questions/16601018/angularjs-ng-model-not-binding-to-ng-checked-for-checkboxes)
* [AngularJs doesn't bind ng-checked with ng-model](http://stackoverflow.com/questions/14226439/angularjs-doesnt-bind-ng-checked-with-ng-model)
* [How to bind ng-model to ng-checked boxes](http://stackoverflow.com/questions/19143037/how-to-bind-ng-model-to-ng-checked-boxes)
* [ng-model 和 ng-checked 的关系](http://plnkr.co/edit/?p=preview)
