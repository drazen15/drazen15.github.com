---
layout: post
title: "坑爹的WordPress"
date: 2013-03-30 20:37
comments: true
tags:
- WordPress
- Octopress
- GitHub
- Summary
- Blog
- Markdown
categories: Thinking
---
周末的时候写了一篇新的博客，发表在我原来的[wangruoyu.wordpress.com](http://wangruoyu.wordpress.com)上面，结果发现我的博客被WordPress的团队给关闭了，具体的原因如下：  

![](/images/WordPress.png)

很蛋疼，我用博客只是记录一下我的想法而已，从来没有WordPress所说的违规行为。搜索了一下之后，发现有很多人和我一样的问题，然后我按照它的只是进行了申诉，但是一直没有回音，放弃了。

之前想过自己搭一个独立博客，但嫌麻烦放弃了，正好借这次机会自己搭一个博客，网上也有比较成熟的方案。我最终选择了同事推荐的GitHub+Octopress的方案，这个方案有几个优点很适合我：

* 管理方便，所有的代码托管在GitHub，只需要会一点前端的知识就好
* 空间大，一篇MrakDown格式的文件最多几K，而GitHub提供了1G的空间。
* 可以使用独立域名
* 不必担心被托管方随意的关掉

我参照一篇[博客](http://firestudio.cn/blog/2013/01/05/ru-he-tong-guo-github-yu-octopress-lai-da-jian-zi-ji-de-bo-ke/)的教程一步一步的搭建，这个过程中还是发生了很多问题，导致反复安装。  

### 1. 支持系统的版本匹配 ###

我的电脑系统是Windows 7 64位，所以下载的Ruby和DevKit全部都是最高版本的64位软件，之后发现各种安装不成功，查询了安装文档后发现，Octopress只支持一部分版本的Ruby。这个问题其实一开始可以通过查询英文文档来避免的。

### 2. 反复安装的过程 ###

在重新安装Ruby和DevKit的过程中，直接从这一步开始：  

![](/images/code1.png)

而忽略了之前的执行`ruby dk.rb init`和`ruby dk.rb install`这一环节。导致后续的DevKit插件安装不成功。这是一个菜鸟级别的错误。

### 3. 忽视了反馈中的信息 ###

没有仔细阅读命令行执行后的反馈信息，所以不知道接下来怎么做。

这次搭建博客的过程中，收获还是很大的。应该在搭建过一两次之后就会熟悉整个流程了。接下来研究一下博客模板、title、分类、标签等问题。