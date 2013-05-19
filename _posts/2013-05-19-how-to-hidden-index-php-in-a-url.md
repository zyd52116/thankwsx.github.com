---
layout: post
title: 如何在url中隐藏动态网址的index.php
---

### 如何在url中隐藏动态网址的index.php
{% highlight apacheconf %}
<IfModule mod_rewrite.c>
RewriteEngine on

#不显示index.php

RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule ^(.*)$ index.php/$1 [QSA,PT,L]

</IfModule>
{% endhighlight %}

{% highlight javascript %}
alert(1);
{% endhighlight %}

http://www.5idev.com/p-thinkphp_htaccess_rewrite.shtml