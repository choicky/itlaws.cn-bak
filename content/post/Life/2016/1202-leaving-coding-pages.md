+++
categories = [
  "IT",
  "Life",
]
date = "2016-12-02T23:45:21+08:00"
title = "停用coding-pages"
tags = [
  "Github Pages",
  "Coding Pages",
]

+++

前两天刚折腾好[在github与coding部署hugo](http://itlaws.cn/post/life/2016/1130-github-coding/)，国内的访问解析到coding.me，国外解析到github.io。

看起来一切都很完美。

但是，今晚发现国内和境外访问时都遭遇了`404`，页面未找到。

Github Pages 遭遇404，我后来知道了原因，是push静态页面时，把`CNAME`文件删除掉了，所以域名解析有问题。
update on 2016-12-03：把 CNAME 文件放在 hugo 根目录的 static 文件夹内，每次生成静态文件时就能重新在 public 文件夹生成 CNAME 文件了。


Coding Page遭遇404，我就百思不得其解了。感觉就是coding.net不稳定导致的。

所以，还是逃离coding.net好了，保留Github Page，也就是 [choicky.github.io](http://choicky.github.io)。