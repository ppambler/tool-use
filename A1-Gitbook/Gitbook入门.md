# Gitbook入门

## ★准备一些工具

- 安装Node.js「GitBook 依赖 Node.js 环境，所以必须要安装 」

  检查是否安装成功：

  ```bash
  node -v
  ```

  返回：

  ```bash
  v6.9.2
  ```

  

- 安装 GitBook 命令行工具

  ```bash
  $ npm install gitbook-cli -g
  ```

  此命令可以用来更新gitbook命令行工具 ，即「升级」

  有了该工具即可以创建多个电子书 

  这里的cli是命令行之意

  检查是否安装成功：

  ```bash
  $ gitbook -V
  ```

  返回：

  ```bash
  CLI version: 2.3.2
  GitBook version: 3.2.3
  ```

## ★新建GitBook项目

1. 选择一个合适的位置，新建一个目录，如「MyBook」 
2. 进入该目录
3. 初始化目录
4. 目录初始化后会出现两个基本文件「README.md」和「SUMMARY.md」

------

操作如下：

```bash
mkdir MyBook #新建目录
cd MyBook    #进入目录
gitbook init #初始化目录
```

## ★编辑电子书内容

1. 知道`SUMMARY.md`这个文件是用于组织整个内容的目录

2. 开始按照你看的书本目录，由此一一对应的创建相应的目录和文件，然后书写你的笔记即可

3. 写完后，就编辑 `SUMMARY.md`这个文件，把对应的目录和文件链接给写上即可

   就像是这样：

   ```markdown
   # Summary
   
   * [简介](README.md)
   * [常见问题](Faq.md)
   ```

   缩进的话，直接像下面这样就可以了

   - 我是标题
     - 我是子标题
       - 我是孙子标题

## ★预览电子书

内容书写完后就直接这样就可以在本地浏览器里预览了：

```bash
gitbook serve
```

不是 `server`，此命令的执行机制：

> 会首先调用 `gitbook build`编译书籍，完成以后会打开一个 web 服务器，监听本地 4000 端口，在浏览器中输入`http://localhost:4000`，即可打开电子书。 

注意：win7很有可能会报错哦！

错误很有可能是这样的 `Error: ENOENT: no such file or directory, stat……`

查阅了[这个](https://github.com/GitbookIO/gitbook/blob/3.2.2/lib/output/website/copyPluginAssets.js#L112)

需要更改这个文件：

`C:\Users\Administrator\.gitbook\versions\3.2.3\lib\output\website\copyPluginAssets.js`

把它的112行`confirm: true `改为 `confirm:false`即可

为什么改这个？我也不知道，看不懂英文:smile:

## ★发布电子书

当电子书内容制作好后，可以使用如下命令，生成html版本的电子书： 

```bash
gitbook build
```

该命令会在当前文件夹中生成`_book`文件夹，用户可以将这个文件夹内容托管到网上，从而实现内容的发布。 

## ★参考资料

- [GitBook 学习笔记](http://yangjh.oschina.io/gitbook/)

## ★一些注意事项

- GitBook的目录，限定为三级 

- 用户可以通过使用标题或者水平分割线标识将GitBook目录分为几个不同的部分 

- 使用链接的语法是这样的 `[]()`，如果圆括号的url也有圆括号的话，你就得这样做才会显示正常：

  ```markdown
  #这是行内式的链接地址
  [Journal of Communication](http://onlinelibrary.wiley.com/journal/10.1111/(ISSN)1460-2466)
  #正确姿势：改为参考式的地址
  [Journal of Communication][1]
  [1]: http://onlinelibrary.wiley.com/journal/10.1111/(ISSN)1460-2466
  ```

  