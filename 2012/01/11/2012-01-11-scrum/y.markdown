---
layout: post
title: Launchy Pro
date: 2013-03-18 13:48
comments: true
tags:
- iOS
- Productivity
- Launch
categories: Life
---
iOS系统比较蛋疼的就是文件夹，对于我这样一个有整理洁癖的人来说，iOS上的App管理非常的不方便，一个文件夹可以放的App数量有限，如果我有很多同一类的App，一个文件夹放不下是让我很头疼的事情，另一方面，很多个文件夹搜索起来也是很费力的。而且一直不习惯手机上的键盘输入，打字效率很低，所以springboard的作用也无从发挥。

后来发现了Launchy Pro这个应用，一见倾心，马上购买。使用之后发现果然是神奇。现在我将Launchy Pro放在doc上面，然后其他的App随意分文件夹，只要通过Launchy管理就好，效率非常高。

Launchy的可扩展性非常高，根据个人的使用习惯可以有不同的组合。目前大部分应用都已经支持url scheme，可以添加进入Launchy，少部分国内的应用还是没有支持。不过我们可以通过手动添加的方式将一些应用加入Launchy。

如何找到App的url scheme?

* 首先可以Google一下,关键词为 `App name`+`url`+`scheme`
* 在[Handleopenurl](http://handleopenurl.com/scheme)上查找
* 通过其他的方法,比如说网易新闻客户端,在找了很长时间无果之后,我返回网易新闻客户端的首页,找到了以下几个关键词:  
	* 手机下载链接: `http://3g.163.com/\newsapp`,关键词:`newsapp`
	* 下载的安卓apk文件,关键词:`netease_newsreader`  
由此我可以推出4个url scheme,一个一个试下来,最后正确的是:`newsapp://`

以上是非官方获取url scheme的方法.

我亲测可用的url scheme：

* 网易新闻客户端: `newsapp://`
* 淘宝客户端: `taobao://`
* wunderlist客户端: `wunderlist://`
* 知乎客户端:`zhihu://`

Trello官方回复说近期内会加上url scheme.