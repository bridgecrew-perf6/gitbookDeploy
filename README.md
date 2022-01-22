# Introduction

## 依赖安装
- gitbook install
    - 

## 启动项目
1. gitbook serve
   1. 会在项目根目录下面生成 _book文件夹（里面是html静态文件）。并且启动了一个web服务器。 访问http://localhost:4000就可以看到效果


## 构建项目
1. gitbook build
   1. 会在mybook目录下面生成 _book文件夹（里面是html静态文件）。如果自己有web服务器，把_book文件夹复制到自己的服务器下面即可（首页是_book文件夹中的index.html）

## gitbook项目插件
1. gitbook项目添加、安装插件方式：book.json文件 在"plugins"中追加插件项，在"pluginsConfig"中进行配置
   1. book.json plugins中追加插件项后 启动项目后会报错，命令行中执行"gitbook install"方可正常运行
         1. 错误信息：`Error: Couldn't locate plugins ${插件名称}, Run 'gitbook install' to install plugins from registry.`
2. book.json中使用的插件
   1. search-pro：高级搜索
   2. anchor-navigation-ex-toc：为文章增加锚点目录栏及回到顶部功能
   3. splitter：扩展导航侧边栏，支持宽度可调节
   4. expandable-chapters-small：章节导航支持多层目录，并配置箭头图标，点击箭头才能实现收放目录
   5. insert-logo：左侧导航栏上方插入Logo

## markdown语法
- 插入图片：![alt text](http://path/to/img.jpg)
  - 图片链接地址可以使用 base64 --> ![alt text][base64Variate]，base64Variate为定义在当前文件最下方的变量 值为图片对应的base64
- 文字链接：[Title](超链地址)
- 插入图片，同时图片加链接：[![alt text](http://path/to/img.jpg)](超链地址)

