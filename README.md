# qs-cookie 


[![Build Status](https://travis-ci.org/dreamstu/cookie.svg?branch=master)](https://travis-ci.org/dreamstu/cookie)
[![spm version](http://spmjs.io/badge/qs-cookie)](http://spmjs.io/package/qs-cookie)

一套方便灵活的高可用的前端组合框架，cookie操作组件

---

## Install

```
$ spm install qs-cookie --save
```

## Usage

```js
var qsCookie = require('qs-cookie');
// use qsCookie
```


---
## 属性概要

### cookie

`释义`
cookie操作对象。

cookie.get(name) *String*

`释义`
获取指定名称的cookie值

`参数及返回`
>@return {String} 获取到的cookie值


cookie.remove(name, domain, path) *String|String|String*

`释义`
删除指定cookie,复写为过期

`参数及返回`
>@param {String} name cookie名称

>@param {String} domain 所在域

>@param {String} path 所在路径


cookie.set(name, value, domain, path, hour) *String|String|String|String|Number*

`释义`
设置一个cookie

>@param {String} name cookie名称

>@param {String} value cookie值

>@param {String} domain 所在域名

>@param {String} path 所在路径

>@param {Number} hour 存活时间，单位:小时

>@return {Boolean} 是否成功


---


### localStorage

`释义`
localStorage操作对象。


localStorage.clear()

`释义`
清空 localStorage


localStorage.getItem(name)

`释义`
根据名字读取值

`参数及返回`
>@param {String} name

>@return {String}


localStorage.isSupports()
`释义`
判断是否支持 localStorage


localStorage.removeItem(name)
`释义`
根据名字移除值

`参数及返回`
>@param {String} name


localStorage.setItem(name, value)
`释义`
设置一个localStorage

`参数及返回`
>@param {String} name

>@param {String} value