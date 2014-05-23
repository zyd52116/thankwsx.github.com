---
layout: post
title: 开发一个chrome扩展
excerpt: 讲述开发chrome扩展的概要细节
---


1. 创建一个manifest.json文件（这点和android开发类似）
```javascript
	{
	  "manifest_version": 2,
	  "name": "Thankwsx`s first Extension",
	  "description": "This extension demonstrates a browser action.",
	  "version": "1.0",
	  "permissions": [
	    "http://thankphp.net"
	  ],
	  "browser_action": {
	    //"default_icon": "icon.png",
	    //"default_popup": "popup.html"
	  }
	}
```

2. 进入chrome的工具->扩展页面，勾选开发者模式，加载未打包扩展。选中manifest.json文件所在目录。

```
你应该已经注意到了，代码中browser_action中有两行已经被注释掉了，就是为了以最快的速度让你入门。
```

