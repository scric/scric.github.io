---
layout: post
title: "搭建个人博客：GitHub + SourceTree"
excerpt: 20分钟搭建个人博客
date: 2017-06-11 08:16:54
tags: Blog
category: Blog
---

* content
{:toc}

网上有一大堆教你如何借助 GitHub 和一系列 Hexo 或者 Jekyll来搭建个人博客的教程  

搭建这样的博客无需租用服务器，也可以不用购买域名，步骤也较比手工建一个网站简单。这是它的优点所在。  

我在这里，不是想重复造轮子，只是给你介绍一种新的方法。

**注意：直接点击蓝色部分可直接跳转到相关网页。**

## 方法

先快速浏览一下下面两个链接里的文章，它们会让你对搭建 Hexo 驱动或者 Jekyll 驱动的博客有一个大致的了解。

你可以先不用去操作，只需了解一下过程和它们之间的相同点即可。

### 注意

在阅读过程中要特别注意: 

+ Framework 的基本结构（各种文件和模块的作用）
+ Markdown 的语法
+ 域名的购买和绑定（可选）
+ 最好把相关链接都打开并保存留给后面再看。

## 文章： 

[小白独立搭建博客 --Github Pages 和 Hexo 简明教程][1]  

[使用 Github Pages + Jekyll 建独立博客][2]

## 操作部分：

### 准备部分：

0、下载一个 [FQ 利器：Lantern][3]

https://github.com/getlantern/forum/issues/833

> 蓝灯是一个能够帮你突破网络限制的工具，它在下面的过程中比如下载工具，访问国外网址有着重要作用，你也可以使用蓝灯来访问 Google 等网站。

1、注册一个 [Github][4] 账户：

https://github.com/

> GitHub 是一个网络仓库，在这里你可以随时随地管理你上传到云端的代码。

2、安装 [Git][5]

https://git-scm.com/downloads

如果被墙：看 [这里][6]

http://pan.baidu.com/s/1miFRKww

> Git 是搭建环境所必需的。

3、 安装 [SourceTree][7]

https://www.sourcetreeapp.com/

如果被墙：看 [这里][8]

http://pan.baidu.com/s/1mhGXzq4

安装完后要注册，否则无法进行下一步。不想注册可以直接使用我的账户。

944242310@qq.com

whosyourdaddy7983

注意：

- 在登陆成功的时候要稍微等一会直至弹出的窗口消失

- 选择跳过初始设置

- No

- 我不想使用 Mercurial
  

> SourceTree 是一款 GitHub 的可视化客户端，我们主要用它来 下载我们上传到 GitHub 的博客和推送更新文章到 Github 上。有了它，我们就可以更方便地使用 GitHub。

## 搭建博客部分

### 挑选一个模板

找一个你中意的博客，我找了两个，可以挑选一下

一个较为简单，只需修改一下博客名和图标就可直接使用，这个是我以前用的。

模板

[Github-Pages-Example-easy][9]

成品实例：

[Beiyuu.com][10]

一个较为复杂，自定义程度高，而且没有纯洁版，要大量修改。后续会更新一篇文章专门介绍这个博客的模板，这也是目前我在用的

模板和成品实例

[gaohaoyang.github.io][11]

### 具体操作

先介绍第一种。

步骤：

- 点开 [Github-Pages-Example-easy][12] 

- 点击右上角的 Fork 

- 跳转完后点击 Setting 

- 将 Repository name 修改为 yourusername.github.io （yourusername 指的是你的用户名，比如我的就是 scric.github.io）

- 点击 Code，然后再点击 Clone and download 

- 复制 框框中的网址并打开 SourceTree 
- 在SourceTree中，点击＋号  ->  Clone -> 将网址黏贴进第一个方框中
- 在第二个方框中点击 Borwse 选择仓库的位置，第三个方框是给仓库命名
- 点击 克隆
- 检验是否搭建成功，在浏览器访问栏中输入 yourusername.github.io ，看是否转到该网址。

## 使用部分

博客搭起来之后，最主要的还是写博客。

首先是文章的名称，它的命名有严格的规定，必须是 2012-02-22-artical-title.MARKUP 这样的形式，MARKUP  是你所使用标记语言的文件后缀名，在这里被设置为 .md 。

所以你应该的形式是 2012-02-22-artical-title.md 。

文章的日期和标记语言后缀与文章的标题的独立的。

然后是文章位置。

放在 _posts 文件夹下。

具体请看

[Beiyuu 博客使用手册][13]

ok 了之后再进入 SourceTree 中进行推送就 OK 了。将页面转到文件状态，将所有修改文件暂存上去，将立即推送变更到 xxx 的选项勾上，然后再进行推送，其间可能会让你登陆 Github 账户，登陆一下就 OK 了。

在另一台电脑上测试，总共只用了 20 分钟不到，就已经实现搭建博客，推送文章到博客这些步骤，还包括了下载文件的时间。

可能是我熟练度高的原因。

## 优点

主要的优点是

+ 不需要加载 ssh
+ 环境只需下载 git 就行了， 没必要再下载 Node 和其他环境
+ 在本地操作
+ 操作可视化，推送只需要在 SourceTree 下操作就 ok 了，更简单和直白，当然你也可以不用下载 SourceTree ，使用 git 命令也可以做到。

## 缺点

主要的缺点有：

+ 较其他教程要多学习一个 SourceTree

## 下期更新

下期更新会更新一篇文章专门介绍该博客模板的结构和语法

在那里你会学到如何自定义你的博客

比如：

+ 修改博客名称和 icon
+ 修改各页面的名称及组件
+ 增删标签页和标题语等等
+ ...

如果你等不及，可以在本地的文件中自行探索，一般在 _config.yml ，index.md ，404.html 中修改



## 参考链接：

1. [小白独立搭建博客 --Github Pages 和 Hexo 简明教程][14]  
2. [使用 Github Pages + Jekyll 建独立博客][15]
3. [FQ 利器： Lantern][16]
4. [gaohaoyang.github.io][17]
5. [Beiyuu 博客使用手册][18]
6. [SourceTree的使用][19]
7. [Markdown 语法][20]
8. [Git 常用命令总结][21]
9. [jekyll Sites][22]
10. [jekyll Docs][23]

如果有其他问题，可以 发邮件反馈

944242310@qq.com



  [1]: https://my.oschina.net/ryaneLee/blog/638440
  [2]: http://beiyuu.com/github-pages
  [3]: https://raw.githubusercontent.com/getlantern/lantern-binaries/master/lantern-installer.exe
  [4]: https://github.com/
  [5]: https://git-scm.com/downloads
  [6]: http://pan.baidu.com/s/1miFRKww
  [7]: https://downloads.atlassian.com/software/sourcetree/windows/ga/SourceTreeSetup-2.0.20.1.exe?_ga=2.72239507.1428932122.1497108054-422389313.1497108054
  [8]: http://pan.baidu.com/s/1mhGXzq4
  [9]: https://github.com/beiyuu/
  [10]: http://beiyuu.com/
  [11]: http://gaohaoyang.github.io
  [12]: https://github.com/beiyuu/
  [13]: http://beiyuu.com/github-pages
  [14]: https://my.oschina.net/ryaneLee/blog/638440
  [15]: http://beiyuu.com/github-pages
  [16]: https://raw.githubusercontent.com/getlantern/lantern-binaries/master/lantern-installer.exe
  [17]: http://gaohaoyang.github.io
  [18]: http://beiyuu.com/github-pages
  [19]: http://jingyan.baidu.com/article/c45ad29cdf274e051753e22c.html
  [20]: http://www.appinn.com/markdown/
  [21]: http://www.cnblogs.com/mengdd/p/4153773.html
  [22]: https://github.com/jekyll/jekyll/wiki/Sites
  [23]: https://jekyllrb.com/docs/home/