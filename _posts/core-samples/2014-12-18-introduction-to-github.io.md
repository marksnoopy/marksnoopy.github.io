---
layout: post
category : 
tagline: ""
tags : [github, jekyll, ruby, DevKit]
---
{% include JB/setup %}

### 写在前面

之前一直在 Evernote 上写东西，通过 twitter 或者 fb 分享，碰巧看到了 github.io，觉得很不错，于是就开始搭建自己的 github page ，中间遇到一些问题，分享出来，算作是第一篇博文吧。

### 什么玩意

github.io ( github page) 是什么，就不多做说明了，不了解或者不明白的可以参见 [官网](https://pages.github.com/) 的说明。

### 安装过程
1 **创建 github.io 库**

官方已经说的很清晰，可以参见[这里](https://pages.github.com/)

2 **快速建立站点**

推荐 [jekyllbootstrap](http://jekyllbootstrap.com/)

3 **安装 jekyll**

环境： 64 bit win7

(1) 安装 ruby 和  devkit

[下载地址]( http://rubyinstaller.org/downloads/)

我选择的是 [Ruby 2.1.5(x64)](http://dl.bintray.com/oneclick/rubyinstaller/rubyinstaller-2.1.5-x64.exe?direct) 和 [DevKit-mingw64-64-4.7.2-20130224-1432-sfx.exe
](http://cdn.rubyinstaller.org/archives/devkits/DevKit-mingw64-64-4.7.2-20130224-1432-sfx.exe)

(2) 把 ruby 加入 PATH

(3) 更新 gem

> gem update --system

(4) 安装 jekyll

> gem install jekyll

由于 ruby 默认的源头是 https://rubygems.org/ ，速度较慢，且可能存在签名问题，所以建议大家切换到 taobao 的源，具体如下：

> gem sources --remove https://rubygems.org/ 

> gem sources -a http://ruby.taobao.org/

(5) 启动 jekyll 服务

切换目录到 *快速建立站点* 中 clone 下来的目录，执行如下命令

> jekyll serve

在这个地方会出现可能会出现两个错误：

a.  Cannot load such file — hitimes/hitimes when installing jekyll

把 hitimes 重新装了以后，发现问题解决了，但具体原因不详，怀疑是版本的问题。

> gem uninstall hitimes

> gem install hitimes

b. 不记得了


(6) 运行

访问 http://localhost:4000


