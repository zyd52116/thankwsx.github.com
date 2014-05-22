---
layout: post
title: 如何在url中隐藏动态网址的index.php
excerpt: apache设置，在url中隐藏index.php的
tags: [apache,index.php,.htaccess]
---

### 如何在url中隐藏动态网址的index.php

	<IfModule mod_rewrite.c>
	RewriteEngine on

	#不显示index.php

	RewriteCond %{REQUEST_FILENAME} !-d
	RewriteCond %{REQUEST_FILENAME} !-f
	RewriteRule ^(.*)$ index.php/$1 [QSA,PT,L]

	</IfModule>

```javascript
alert(1);
```
http://www.5idev.com/p-thinkphp_htaccess_rewrite.shtml