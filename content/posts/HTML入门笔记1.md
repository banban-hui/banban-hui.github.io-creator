---
title: "HTML入门笔记"
date: 2019-12-24T15:36:53+08:00
draft: false
---

# HTML入门笔记1

## HTML的历史

* 1990年由英国的 Tim Berners-Lee 发明
* 我们的祖师爷就是李爵士
* 最初的HTML一共只有18个元素，最新版的HTML大约由110个标签

## HTML的起手式

* Emmet 感叹好

```html
<!DOCTYPE html>    //文档类型
<html lang="en">   //html标签，可以改成"zh-CN"
<head>
    <meta charset="UTF-8">     //文件字符编码
    <meta name="viewport" content="width=device-width,
    initial-scale=1.0">       //禁用溶放，兼容手机
    <meta http-equiv="X-UA-Compatible" content="ie=edge">//告诉ie使用最新内核
    <title>Document</title>    //标题

</head>
<body>

</body>
</html>

```

## 章节标签
* h1 ~ h6 表示不同等级的标题，h1最高
* section 表示新开启的章节
* p       表示段落
* header  表示头部，如：顶部广告
* footer  表示脚部，如：版权声明"&copy"
* main    表示主要内容
* aside   表示次要内容，如资料来源
* div     表示划分，div包含的内容是一整块

## 全局属性
所有标签都有的属性
* class 给标签分一个类
* contenteditable 使元素在页面可以直接被编辑
* hidden 使元素看不见
* id  给标签分一个id
* style  给元素一个style，js的style优先级最高
* tabindex  控制TAB键的顺序，等于正整数表示顺序，等于0表示最后访问，等于-1表示别访问
* title   显示完整的内容 

## 内容标签
* ol + li 有顺序的列表
* ul + li 没有顺序的列表
* dl+dt+dd 描述列表，dt表示描述的对象，dd 表示描述的内容
* pre 如果你保留内容的多个空格/TAB/换行，就用pre把内容包起来
* hr 分割线
* br  换行
* a   超链接
* em  语气的强调
* strong 本身的强调
* code 包起来的内容字体是等宽的，可用于插入代码，一般要用pre包起来，保留代码的空格和换行
* quote 内行的引用
* blockquote 块的引用，会换行显示
