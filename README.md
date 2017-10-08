---
title: er
date: 2017-10-08 19:35:16
tags:
	- JavaScript
	- 你好
	- 学习
categories:
	- 你好吗
---

# 远程仓库

## git
git 是一个分布式的 版本控制工具，特点，就是版本库存放在本地！！！

## 远程仓库的作用
就是共享版本库！！！ 共享代码！！！

## 远程仓库的创建

***远程仓库其实就是一个裸仓库***

## 裸仓库

创建裸仓库
```
git init --bare
```

裸仓库创建完成之后，就不需要做任何操作了，在裸仓库中不能进行任何的开发操作


## 远程仓库的操作命令
1. 给远程仓库推送内容
```
git push 远程仓库地址 本地分支名称:远程分支名称

如果本地分支名称和远程分支名称相同，那么可以缩写如下：
git push xxx.xxx.git master:master
git push xxx.xxx.git master
```

2. 获取远程仓库中所有的内容
```
git clone 远程仓库地址 文件夹名称

文件夹名称也可以不用写，默认使用的就是远程仓库的文件夹名称！！
```

3. 获取远程仓库中更新了的内容
```
git pull 远程仓库地址 分支名称
```





## 注意
只有在远程仓库中从未推送过任何内容的时候，我们才能随意向里面推送任何内容

但是，一旦已经推送过一次内容了，那么之后就不能随便的向远程仓库推送内容了，能推送的，只能是和第一次推送相关的修改的内容！！


**每次在向远程仓库中推送新内容的时候，必须先进行一次获取更新内容的操作（pull），否则可能推送失败！！！**