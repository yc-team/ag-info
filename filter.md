## filter

* currencyFilter: true,
* dateFilter: true,
* filterFilter: true,
* jsonFilter: true,
* limitToFilter: true,
* lowercaseFilter: true,
* numberFilter: true,
* orderByFilter: true,
* uppercaseFilter: true


#### json

```
{{user | json}}
```

```
function jsonFilter() {
  return function(object) {
    return toJson(object, true);
  };
}
```



* [data-filter](https://docs.angularjs.org/api/ng/filter/date)
* [json filter demo](http://jsfiddle.net/pkozlowski_opensource/ASspB/2/)