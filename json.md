# json
 
## angular.toJson

```
function toJson(obj, pretty) {
  return JSON.stringify(obj, toJsonReplacer, pretty ? '  ' : null);
}


function toJsonReplacer(key, value) {
  var val = value;

  if (/^\$+/.test(key)) {
    val = undefined;
  } else if (isWindow(value)) {
    val = '$WINDOW';
  } else if (value &&  document === value) {
    val = '$DOCUMENT';
  } else if (isScope(value)) {
    val = '$SCOPE';
  }

  return val;
}

```


## angular.fromJson

```
function fromJson(json) {
  return isString(json)
      ? JSON.parse(json)
      : json;
}
```

#### 扩展

* [api fromJson doc](https://docs.angularjs.org/api/ng/function/angular.fromJson)
* [api toJson doc](https://docs.angularjs.org/api/ng/function/angular.toJson)
* [demo](http://jsfiddle.net/pkozlowski_opensource/ASspB/1/)
* [How to use angular.toJson on a angular controller or scope](http://stackoverflow.com/questions/11819301/how-to-use-angular-tojson-on-a-angular-controller-or-scope)