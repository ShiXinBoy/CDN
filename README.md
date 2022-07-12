# 思卿长安归 の CDN

## 前言

CDN源文件托管在github仓库地址为：

``` html
https://github.com/ShiXinBoy/CDN
```
请根据仓库内文件位置调用。

本站分发至多个平台，对于js，css的调用推荐顺序为：

==fastly.sdelivr > cdn.jsdelivr > 其他==

对于图片等资源的引用：

``` html
 https://raw.fastgit.org/shixinboy/CDN/main/
```
==同时 ，你的HTML的head标签内应包含:==

``` html
<meta name="referrer" content="no-referrer"/>
```

## 调用

### 1.jsdelivr调用

链接：
``` html
https://fastly.jsdelivr.net/gh/shixinboy/cdn@latest/
https://cdn.jsdelivr.net/gh/shixinboy/cdn@latest/
```
> 请使用==@version==指定版本号，若调用最新请使用==@latest==
>
> 注意:该链接调用支持jsdelivr链接参数，
>
> 已有版本([版本号更新内容](#更新内容)):
>
> @2.2.0
### 2.自建托管调用

链接: 
``` html
https://sxcdn.vercel.app/
https://sxcdn.netfily.app/
```
> 以上托管平台不支持版本调用，默认同步仓库最新内容（即使是未发布tag的小文件修改）

### 3.raw调用

```html
https://raw.githubusercontent.com/shixinboy/CDN/main/
https://raw.githubusercontents.com/shixinboy/CDN/main/
```

> raw用于引用静态资源，无法指定版本。国内请使用第二个链接。第一个链接为github原始链接

## 更新内容

2022年7月7日：v2.2.0

> 添加live2d
> 添加fa图标库

---


<center class="div">
    Powered By <a href="https://shixin.vercel.app">思卿长安归</a>
    <br>
    Copyright © 2021 - 2023 思卿长安归 All Rights Reserved
</center>


