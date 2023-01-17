#h5ai----搭建私有云
=================
[官网链接](https://larsjung.de/h5ai/)
-----------------
##h5ai
-----------------
现代HTTP Web私有云

h5ai是HTTP Web服务器的现代文件索引器，专注于您的文件。目录以吸引人的方式显示，浏览它们会通过不同的视图、面包屑和树木概述来增强。最初h5ai是HTML5 Apache索引的首字母缩略词，但现在它也支持其他Web服务器。

查看启用了大多数功能的[演示目录](https://larsjung.de/h5ai/demo/)。一个简化的例子和我的实际用例是此页面上项目的发布目录。

需要PHP 7.0+，并且可以与Apache httpd、lighttpd和nginx配合使用。使用最新版本的基于Chromium的浏览器、Firefox、Safari和Edge的最佳用户体验，但如果禁用了JavaScript，则为旧浏览器提供静态回退。

##精选
-----------------
有很多可选的扩展和配置选项来自定义目录列表的网络外观。所有标记都是有效的HTML5，带有CSS3和最好的JavaScript，以构建一个新鲜但最小的用户界面和专注于文件的用户体验。

一些可选功能是：文件排序、不同视图模式、本地化、面包屑、树视图、自定义页眉和页脚、文件过滤器和搜索、文件夹大小、自动刷新、打包下载、二维码、缩略图、文件预览

##安装
-----------------
```
1. 将文件夹_h5ai复制到Web服务器的文档根目录：DOC_ROOT/_h5ai。

DOC_ROOT
 ├─ _h5ai
 ├─ your files
 └─ and folders

2. 访问http://YOUR-DOMAIN.TLD/_h5ai/public/index.php，检查是否可以访问h5ai。此页面显示了有关服务器功能的一些提示。
3. 添加/_h5ai/public/index.php（注意领先的斜杠！）到默认索引文件列表的末尾。通过这种方式，h5ai将管理DOC_ROOT中和下方没有索引文件的所有目录。

Apache httpd 2.2/2.4：例如在httpd.conf或根目录的.htaccess文件集中：

DirectoryIndex  index.html  index.php  /_h5ai/public/index.php

nginx 1.2：例如，在nginx.conf：

index  index.html  index.php  /_h5ai/public/index.php;
```

##配置
-----------------
```
主要配置文件是_h5ai/private/conf/options.json。您可能想要更改一些记录的设置。但_h5ai/private/conf中还有一些文件，你可以看看。
```
