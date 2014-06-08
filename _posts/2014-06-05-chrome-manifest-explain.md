---
layout: post
title: Chrome扩展声明文件解释manifest.json
excerpt: 简要介绍现有chrome扩展源码中的声明文件manifest.json
---

参考资料：
- http://open.chrome.360.cn/extension_dev/manifest.html
- https://developer.chrome.com/extensions/manifest

	{
		"manifest_version":2,	//必须，且目前是固定的版本（2014）
		"name":"扩展名称",
		"version":"扩展版本号",
		//以下为推荐项
		"default_locale":"en",	//默认扩展语言，作用待定
		"description":"对于扩展作用的描述",
		"icons":{},
		//很关键
		//书签栏功能icon的配置
		"browser_action":{},
		//地址栏功能icon的配置
		"page_action":{},
		//可选配置
		"author":"作者",
		"automation":"",
		"background":{},
		"background_page":"",
		"chrome_setting_overrides":{},
		"chrome_ui_overrides":{
			"bookmarks_ui":{
				"remove_bookmark_shortcut":true,
				"remove_button":true
			}
		},
		"chrome_url_overrides":{},
		"commands":"",
		"content_pack":"",
		"content_script":"",
		"content_security_policy":"",
		"convert_from_user_script":"",
		"current_locale":"",
		"devtools_page":"",
		"externally_connectable":{
			"matches":["..."]
		},
		"file_browser_handlers":[],
		"homepage_url":"",
		"import":"",
		"incognito":"spanning|split",
		"input_components":"",
		"key":"",
		"minimum_chrome_version":"",
		"nacl_modules":[],
		"oauth2":"",
		"offline_enabled":true,
		"omnibox":{
			"keyword":""
		},
		"optional_permissions":"",
		"options_page":"",
		"page_actions":"",
		"permissions":[],
		"platforms":"",
		"plugins":"",
		"requirements":{},
		"sandbox":[],
		"script_badge":"",
		"short_name":"",
		"signature":"",
		"spellcheck":"",
		"storage":{
			"managed_schema":""
		},
		"system_indicator":"",
		"tts_engine":"",
		"update_url":"",
		"web_accessible_resources":[]

	}
