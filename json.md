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

#### 扩展

* [api doc](https://docs.angularjs.org/api/ng/function/angular.fromJson)
* [demo](http://jsfiddle.net/pkozlowski_opensource/ASspB/1/)