% 主题：我的一天
% Felix
% 2020-03-13

# 我的一天

王东斌

2020.6.24

# 早晨

## 起床

- 关闭闹钟
- 从床上爬起来

## 吃早餐

- 鸡蛋
- 牛奶

# 晚上

## 吃晚餐

- 吃烧鸡
- 喝茅台

------------------

没有标题

我被强制了

## 睡觉

- 上床
- 入睡

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

