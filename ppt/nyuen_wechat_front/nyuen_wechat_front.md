# 恩元公众号前端项目

王东斌

2020.6.28

# 项目简介

## 交互流程
![avatar](http://i2.tiimg.com/722130/727f31bb85495a86.png)


## 框架／库

- vue
- vuex
- vue-router
- element-ui
- axios

## 目录结构

- src

# Vue-router前端路由

## 路由

```
//insert

```

## 路由守卫

```
//insert

```

# Vuex状态管理
## index

```
//insert

```

## getter

```
//insert

```

## module

```
//insert

```

# axios及api请求封装
## axios封装

```
//insert

```

## api请求

```
//insert

```

# element-ui使用
## el-form表单

```
//insert

```

## $alert提示

```
//insert

```

# mock+koa2假数据
## koa2（nodeJS框架）做服务

```
//insert

```

## mock制作假数据

```
//insert

```

# END

感谢各位的观看




# 代码

## 代码标题2-1

```
//不同的目录请修改basic_url地址
    var basic_url = '../../reveal.js/'
	function dynamicLoadCss(url, params) {
        var head = document.getElementsByTagName('head')[0];
        var link = document.createElement('link');
        link.type='text/css';
        link.rel = 'stylesheet';
        link.href = basic_url + url;
        if(params){
        	for(var key in params){
        		link[key] = params[key]
        	}
        }
        head.appendChild(link);
    }
    function dynamicLoadJsArr(urls, callback) {//所有的都加载完成,执行callback
        var head = document.getElementsByTagName('head')[0];
        var tags = []
        for(var url of urls){
        	tags.push(false)
        	var script = document.createElement('script');
        	script.type = 'text/javascript';
        	script.src = basic_url + url;
	        if(typeof(callback)=='function'){
	            script.onload = script.onreadystatechange = function () {
	                if (!this.readyState || this.readyState === "loaded" || this.readyState === "complete"){
	                	tags.unshift(true)
	                	tags.pop()
	                	var res = tags.every(function(item){
	                		return item
	                	})
	                	if(res){
	                		callback()
	                		script.onload = script.onreadystatechange = null
	                	}
	                }
	            };
	        }
	        head.appendChild(script);
        }
    }
```

## 代码标题2-2

```
//不同的目录请修改basic_url地址
    var basic_url = '../../reveal.js/'
	function dynamicLoadCss(url, params) {
        var head = document.getElementsByTagName('head')[0];
        var link = document.createElement('link');
        link.type='text/css';
        link.rel = 'stylesheet';
        link.href = basic_url + url;
        if(params){
        	for(var key in params){
        		link[key] = params[key]
        	}
        }
        head.appendChild(link);
    }
    function dynamicLoadJsArr(urls, callback) {//所有的都加载完成,执行callback
        var head = document.getElementsByTagName('head')[0];
        var tags = []
        for(var url of urls){
        	tags.push(false)
        	var script = document.createElement('script');
        	script.type = 'text/javascript';
        	script.src = basic_url + url;
	        if(typeof(callback)=='function'){
	            script.onload = script.onreadystatechange = function () {
	                if (!this.readyState || this.readyState === "loaded" || this.readyState === "complete"){
	                	tags.unshift(true)
	                	tags.pop()
	                	var res = tags.every(function(item){
	                		return item
	                	})
	                	if(res){
	                		callback()
	                		script.onload = script.onreadystatechange = null
	                	}
	                }
	            };
	        }
	        head.appendChild(script);
        }
    }
```

