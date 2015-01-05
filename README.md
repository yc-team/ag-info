ag-info
=======

ag info


规范：

1、命名：

> SpicyController is just a plain JavaScript function. As an (optional) naming convention the name starts with capital letter and ends with "Controller".

地址：https://docs.angularjs.org/guide/controller





## 指令：

directive()方法：
传入一个字符串和一个函数来注册一个指令。
字符串是指令的名字，指令名应该是驼峰命名
函数一个返回一个对象

返回的对象中包含了用来定义和配置指令所需的方法和属性。

> 比如html使用 my-directive声明指令，指令定义必须以myDirective



* restrict

> 限制directive为指定的方式

1、A  属性，默认值 <div my-directive="exp"></div>
2、E  元素  		 <my-directive></my-directive>
3、C  class      <div class=”my-directive:exp;”></div>
4、M  注释        <!-- directive: my-directive exp -->


* replace

> 默认情况下，将模板生成的HTML代码嵌套在自定义标签内部，可以设置replace


ng-include






provider()  为服务注册提供者，2个参数：

1、name 在providerCache中是注册的名字。 name+Provider会成为一个服务的提供者，name也是服务的实例
2、aProvider 
如果是函数，会通过依赖注入被调用，并负责通过$get方法返回一个对象


返回一个已经被注册的提供者实例，必须返回一个定义有$get()函数的对象，否则报错。




constant() 将一个已经存在的变量值注册为服务，并将其注入到应用的其他部分当中。

1、name  需要注册的常量的名字
2、value 需要注册的常量的值

返回一个注册后的服务实例

不会被装饰器拦截




控制器：

命名首字母大写，然后加Controller




拦截器：

调用模块的.factory()方法来创建拦截器



ng-include：

其实内部$http.get来获取一个模板
