---
title: "HTML常用标签"
date: 2019-12-25T12:56:28+08:00
draft: false
---

# a标签
## 属性
### href
href 的取值
1. 网址
例：
                 
   https://baidu.com   
   http://baidu.com   
   //baidu.com
```html
<a href="//baidu.com">百度</a>
```
2. 路径    
   /a/b/c.html 以及 a/b/c.html
   例：
```html
<a href="/a/b/c.html">c.html</a>
```
   直接指向文件：index.html以及 ./index.html
   例：
```html
<a href="index.html">index</a>
```

3. 伪协议
  * javascript:; 如果你想做一个没有功能的a标签
```html
<a href="javascript:;">查看</a>
```
  * 加id 
```html
<a href="xxx">查看</a>   //xxx是id
```
 * mailto 邮箱
```html
<a href="xxxx.@126.com">邮箱</a>
```
   * Tel 电话
```html
<a href="189xxxxxxxx">电话</a>
```
### target 
a标签target的取值
* _blank   表示在新的的窗口打页面 例：
```html
<a href="//baidu.com" target="_blank">百度</a>
```
* _self    表示在当前窗口打开页面
* _top     表示在当前窗口的最顶层窗口打开页面
* _parent  表示在操作窗口的上一层窗口打开页面
  
程序员的命名
* window的name
* iframe的name    用于嵌套窗口

# table 标签
## table 里面只有三个东西
1. `<thead></thead>`   表头
2. `<tbody></tbody>`   表体
3. `<tfoot></tbody>`   表尾
4. `<tr></tr>`表行
5. `<th></th>`表标题
6. `<td></td>`表数据

例：下面一个成绩单的表主要代码
```html
<table>
    <thead>
        <tr>
            <th></th>
            <th>小红</th>
            <th>小明</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>语文</th>
            <td>90</td>
            <td>80</td>
        </tr>
        <tr>
            <th>数学</th>
            <td>60</td>
            <td>70</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <th>总分</th>
            <td>150</td>
            <td>150</td>
        </tr>
    </tfoot>
</table>
```
# img 标签
作用：发出get请求，展示一张图片
## 属性
1. alt 加载失败时，可以添加文字提示用户
2. height 高
3. width 宽    注：只写高度，宽度会自适应，反之一样，不让图片变形的方法之一
4. src 图片的地址
## 事件
1. onload/onerror 监听图片是否加载成功

### 使图片在手机上正常显示
```html
<style>
    *{
        margin:0;
        padding:0;
        box-sizing:border-box;
    }
    img{
        max-width:100%;
    }
</style>
```
# form 标签
作用：向后端发出一个请求，刷新页面
## 属性
1. action 请求的地址
2. method 请求的方式get/post
3. autocomplete 输入框有提示输入
4. target 在哪打开页面
## 事件
on submit

### input 和 button 的区别
1. input里面只能传文本
2. button里面可以加其他标签或图片

# input 标签
##常用属性
* test 输入文本
* color 选择颜色
* radio 单选项
* checkbox 复选项
* file 上传单个文件
* `<input type="file" multiple />`上传多个文件
* hidden 看不到的输入框
  
textarea 多行文本输入框

select  多选一

## 事件
onchange

onfocus

onblur 


# 注意事项
1. 一般不监听input的click事件的
2. form里面的input要有name
3. form里面要放一个type=submit才能触发submit事件

