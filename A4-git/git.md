# Git

## ★升级

> 原先的git版本是很低的，为此我打算升级。

**➹：**[How to upgrade to the latest version of Git on Windows? Still showing older version](https://stackoverflow.com/questions/13790592/how-to-upgrade-to-the-latest-version-of-git-on-windows-still-showing-older-vers)

 按照这个答案：

> Since Git 2.16.1(2) you can use
>
> ```
> C:\> git update-git-for-windows
> ```
>
> In versions between 2.16.1 and 2.14, the command was
>
> ```
> C:> git update
> ```
>
> That command does not exist in Git 2.13 and before 

我的是Git 2.13，显然不能使用命令行了。由于360可以升级这个2.13版的，我打算升级后，再使用命令行升级到最新版，结果GG了……也不知道哪里出错了，回滚也不成功了……心里一万头草泥马……早知道就不更新了，这下好了吧！不能用了，没事找事……你看你一折腾又没有完成今天的任务了……

然后我又开始搜索答案了，**➹：**[Git 安装、卸载、升级与配置](https://blog.imzhengfei.com/git-an-zhuang-xie-zai-sheng-ji-yu-pei-zhi/)

根据这个答案，得要卸载当前的Git（我在想卸载了，那么原先的本地仓库会不会也被清了）再安装最新版的……我……哑口无言

我不管了，也不卸载了，直接装最新版的……这次装到C盘

最新版的安装过程和以往的（有个SSL等等……）不同了，我只能根据「芳芳的配置+默认选项」，一路过关，最后安装成功了

我在想之前在旧版配置的数据会失效吗？——没有失效，因为它们都在这个目录下 `Administrator`，不依赖Git的安装目录

看看Git的安装目录：

```
C:\Program Files\Git
```

ps：之前有个 `tree.exe`的命令，所以需要把它拷贝到： `C:\Program Files\Git\usr\bin`这里来

**➹：**[Git Bash tree（windows）让windows支持tree](http://hisen.me/20170713-Git%20Bash%20tree%EF%BC%88windows%EF%BC%89/)、[tree download](http://gnuwin32.sourceforge.net/packages/tree.htm)

如果有时间，那就看看像使用 `tree.exe`那样，找找没有好用的命令行，**➹：** [GnuWin Packages](http://gnuwin32.sourceforge.net/packages.html)

这里是 `GnuWin`，而Git Bash则是 `MINGW64`，这为啥我可以使用 `tree.exe`？它们之间是有什么联系吗？

**➹：**[Cygwin 和MinGW 的区别与联系是怎样的？](https://www.zhihu.com/question/22137175)、[GNU](https://zh.wikipedia.org/wiki/GNU)

> MinGW 是让Windows 用户可以用上GNU 工具 

