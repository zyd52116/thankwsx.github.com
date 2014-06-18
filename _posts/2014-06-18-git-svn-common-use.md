---
layout: posts
title: git svn命令使用流程
excerpt: git svn命令使用流程
---

git安装好之后，已经自带了git svn命令。
```
git svn clone -s SVNPATH 
```
是git svn init 和 git svn fetch的结合。用于从svn仓库拉取源代码，注意命令参数-s
-s的意思是拉取标准svn布局，即基于trunk,branches,tag来拉取，如果只需要拉取指定目录，不提供-s参数即可。

一般该命令视svn库大小持续时间不等，有足够的时间去泡杯咖啡去。