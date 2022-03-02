---
name: 简介
---

# classnotfound.com.cn是如何实现的



## 问题的提出

在开发java应用时，经常遇到ClassNotFoundException错误，意思是的找不到指定的类，有时也会出现NoClassDefFoundError错误，其原因是缺少相应的jar包，或jar包未放到编译程序可识别的目录下。问题的原因很简单，也很好定位，但单纯通过类名去查找缺少哪个jar，还是有一定难度的。有一个国外网站findjar.com，实现了通过类名查找jar的功能，但这个网站可能是由于访问量较大，网站经常打不开，而且访问速度很慢，所以产生了开发类似网站的想法。

经过一段时间的开发和数据整理工作，目前https://classnotfound.com.cn 已上线，源代码已在https://github.com/git-cloner/classnotfound 开源。

https://classnotfound.com.cn 实现按类名和jar包名搜索jar的能力，如果关键字由“.”隔开，则认为是类名，否则为jar包名，检索到jar包可以同时查看历史版本及POM文件。