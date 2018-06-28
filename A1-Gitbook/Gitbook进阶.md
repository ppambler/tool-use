# Gitbook进阶

## 如何把本地的项目上传到github像网页一样浏览？

我们的Gitbook项目，有个叫 `_build`的目录，这个目录是 `gitbook build`输出的一个**静态网站** ，如果你把这个  `init`为一个仓库的话，本地更新会把这个目录删掉再重新生成的，这意味着本地仓库就被删掉了，所以这就很尴尬了啊！

做法：

把整个Gitbook当作是一个仓库，这是个master分支，然后提交到远程仓库。

创建`gh-pages`分支 ，这个分支用于保存html文件的，上面那个是md文件

参考这篇文章：

[发布到github pages](https://yuzeshan.gitbooks.io/gitbook-studying/content/publish/gitpages.html)

我用了下面这篇文章，照葫芦画瓢做了一遍，我不知道分支的名字是否一定要是 `gh-pages`，最终用了这个 `pages`名字，我不知道是不是这个原因，静态页面始终是那个md文件，如何让 `pages` 分支启用 GitHub pages服务呢？

我找不到答案，额……

我要删除这个 `pages`分支吗？

然后再尝试一次？

我想我需要再次看一下关于Git的教程才可以，之前我只会用一些简单的操作，这显然是不够的……

[将_book发布到pages上](http://yangjh.oschina.io/gitbook/UsingPages.html)

ps：`github pages`是Github 的静态页面托管服务