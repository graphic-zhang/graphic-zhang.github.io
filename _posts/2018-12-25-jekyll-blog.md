---
layout: post
title: "关于jekyll搭建个人网站的一些经验"
date: 2018-12-25 22:34:39
categories: [jekyll]
---
[jekyll](https://jekyllrb.com/)
**jekyll**是用Ruby写的一个静态网站生成器，（Ruby是一种很高层次的动态脚本语言，
和Python,PHP,Perl有些类似），所以用到了**gem**(Ruby语言的包管理器，相当于
python对应的pip)以及**bundle**(Ruby依赖库的管理)。
所以如果需要本地编译，注意检查相关的开发环境：
```
   ruby -v
   gem -v
   bundle -v
```
如果只是简单的使用jekyll，则完全不用管本地环境，只要在github搜索jekyll，找到喜欢的实现，fork+clone后，改改_config.yml文件，写好对应的post markdown文件，push到github后，
服务器端自会用脚本编译，进而呈现在个人的github pages上。
如果需要本地编译调试，则需要安装好Ruby环境，再用以下命令，
```
bundle exec jekyll serve
```
或者
```
jekyll serve
```
更加详细的，可以参考[jekyll usage](https://jekyllrb.com/docs/usage/)
###前端开发：
可以记一下这些关键词，W3C，html,css,PHP,静态网站，动态网站，数据库...
也可以观看当前流行网站的架构，比如facebook好像是python+mysql。
这还只是网站，作为一个产品，还有移动端(android,ios),可以说很复杂了。