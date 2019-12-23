---
title: "如何使用hugo在github写博客"
date: 2019-12-23T16:15:48+08:00
draft: false

---

# 如何使用hugo在github写博客

## 需要使用的工具
VSCode + Git + MD + GitHub

## 安装hugo
* [官方教程](https://gohugo.io/getting-started/installing)
  
* Mac安装方式
 ```
 brew install hugo
 hugo version
 ```
* Windows安装方式
1. 在[Hugo releases 页面](https://github.com/gohugoio/hugo/releases)下载hugo_x.xx.x_Windows-64bit.zip
2. 解压，把hugo.exe放在D:\Software\hugo\hugo.exe
3. 把D:\Software\hugo\加到PATH
4. 重启终端，运行hugo version 查看版本


## 快速搭建博客

1. 进入[hugo](https://gohugo.io/)官网，点击Quick Start 快速开始
2. 从Step 2 开始抄代码，直到 Step 7 
3. 得到一个public目录，这就是我们的博客站点
4. hugo server -D 可以预览草稿
5. hugo server 可以预览非草稿
6. 上传到github


* （资料来源：饥人谷）




