---
title: github ssh 相关
date: 2016-07-14 19:53:52
tags:
- ssh免密push
- 技术
- 生活记录
categories:
- javascript
- web
---

### 这一次我准备将我的hexoblog与github远程仓库相衔接,但是我忘掉了一些关键的问题结果,没有成功

#### 1.ssh公钥免密 我们需要在git或者npm中键入 ssh-keygen -t rsa,之后会在你的界面上生成Enter file in which to save the key (/c/Users/Administrator/.ssh/id_rsa):
/c/Users/Administrator/.ssh/id_rsa already exists.,然后敲击回车,一路执行回车,然后会先界面上形成一种冒泡泡的的内容,这表示成功了.
### 记住 (/c/Users/"电脑用户名"/.ssh/id_rsa),这是你公钥文件的所在路径,找到id_rsa.pnb文件,将其内容复制
### 然后登陆你的github账号,点击你的头像,点击settings选项,进入后点击sshandgpgkey,然后点击newsshkey新建在key文件输入框中输入你之前复制好的公钥. 然后就ok,记住title不要填任何东西.
