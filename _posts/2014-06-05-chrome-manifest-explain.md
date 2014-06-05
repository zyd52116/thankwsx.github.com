---
layout: post
title: Chrome扩展声明文件解释manifest.json
excerpt: 简要介绍现有chrome扩展源码中的声明文件manifest.json
---

```javascript
	{
		"manifest_version":2,	//必须，且目前是固定的版本（2014）
		"name":"扩展名称",
		"version":"扩展版本号",

		"default_locale":"en",	//默认扩展语言，作用待定
		"description":"对于扩展作用的描述",
		"icons":{}
	}
```