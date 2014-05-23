---
layout: post
title: 编码中一些容易犯的小错误
excerpt: 大小写，分号，引号，中英文，空格等等稀奇古怪的问题。
---

一个JavaScrtip的object，因为key多写了一个空格，导致一直取不到数据，很低级吧。

```javascript
	var obj = {"key ":"value"};
	console.log(obj["key"]);
```

你运行下代码试试。

再运行下下面这个，这个写对了。

```javascript
	var obj = {"key":"value"};
	console.log(obj["key"]);
```