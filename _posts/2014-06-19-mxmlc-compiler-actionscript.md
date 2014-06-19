---
layout: post
title: mxmlc编译actionscript生成swf
excerpt: 使用FlexSDK中的mxmlc命令生成swf目标文件
tags: [mxmlc,apache flex,fcsh,actionscript,flexsdk]
---

1. 下载FlexSDK
[http://flex.apache.org/download-binaries.html]
2011年 adobe将FlexSDK这个项目捐献给ASF，项目变成Apache Flex
 - 因为Flex协议的变更，有些配置，可以手动简单设置，当然apache提供了installer，不过需要额外下载，手动设置可以让我们更熟悉。

2. 编写ActionScript入口文件
fso.as


~~~ actionscript
package  {
	import flash.display.MovieClip;
	public class fso {
		public function fso() {
			
		}
	}
}
~~~

3. 编写命令脚本
将编译命令单独编写到cmd.txt文件中，以备后续使用，主要是fcsh命令不支持执行上一个命令。

~~~
mxmlc -source-path /PATH/TO/ACTIONSCRIPT/PROJECT -static-link-runtime-shared-libraries=true -show-actionscript-warnings=false /PATH/TO/ACTIONSCRIPT/PROJECT/fso.as -o /PATH/TO/ACTIONSCRIPT/PROJECT/fso.swf
~~~

4. 命令编译
进入fcsh命令，将步骤3中的命令代码拷贝进去，回车执行。

