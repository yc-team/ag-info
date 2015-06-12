## post

## httpProvider

#### transformRequest

对整个 http 的数据格式进行转换设置

```
angular.module('app', [])
.config(['$httpProvider', function ($httpProvider) {
	$httpProvider.defaults.transformRequest = [
		function (request) {
			return $.param(request);
		}
	]
}]);
```



* [post](https://docs.angularjs.org/api/ng/service/$http#post)
* [httpProvider](http://jsfiddle.net/X2p7r/41/)
* [AngularJS, $http and transformResponse](http://stackoverflow.com/questions/18147126/angularjs-http-and-transformresponse)