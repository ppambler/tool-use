# plug-in

## ★Package Control

**➹：**[Installation - Package Control](https://packagecontrol.io/installation)

sublime text 3的安装方式，**✎：**

```python
import urllib.request,os,hashlib; h = '6f4c264a24d933ce70df5dedcf1dcaee' + 'ebe013ee18cced0ef93d5f746d80ef60'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

拷贝这个Python code ，打开sublime text3，使用快捷键 「Ctrl+`」打开需要粘贴的目标位置console，然后回车即可

## ★Emmet

安装这个[蚂蚁](https://github.com/emmetio/emmet)，怎么装呢？看一下这个，**✎：**

**➹：**[Sublime Text 3前端开发常用优秀插件介绍 - 黄映焜 - 博客园](http://www.cnblogs.com/hykun/p/sublimeText3.html)

1. `Ctrl+Shift+P`
2. 输入`ip`，选中这个 `Package Control: Install Package`，然后回车，启动这个需要等个几秒
3. 输入你想要的插件，选择，回车
4. 观察左下角的安装提示，有个`=`在动来动去的话，就是安装进行中；如果安装成功则提示 `successfully`

ps：安装这个插件会自动下载并安装PyV8二进制文件 

常用的快捷键，**✎：**

1. `Ctrl+E`：快速生成html

其它的你就看这个[cheat-sheet](https://docs.emmet.io/cheat-sheet/)好了

## ★其它插件

### ◇安装插件原则

> 插件有很多，但不建议全部都安装，用到那个安装那个，安装过多，由于插件质量良莠不齐，会使软件本身不稳定，经常挂掉。 

补充，到[这里](https://packagecontrol.io/browse)搜索插件，会有该插件的排行榜。搜索到对应的插件后就在本地安装即可！

其实，一下子装那么多插件挺无聊的，不过，可以学英文……因为即便你安装了插件，可是你还得要看它的文档说明是如何使用的啊！

**➹：**[jikeytang/sublime-text: sublime-text](https://github.com/jikeytang/sublime-text)

### ◇感觉不错就安装吧！

1. [SublimeText插件列表](https://sublime.wbond.net/) （最重要）
2. [Side Bar](https://github.com/titoBouzout/SideBarEnhancements)`增强的侧边栏` ，如右击某个文件或目录会发现相较之前多了很多个菜单
3. [Docblockr](https://github.com/spadgos/sublime-jsdocs)`增强js注释` 
4. [Alignment](https://github.com/wbond/sublime_alignment)`等号对齐` 
5. [AutoFileName](https://github.com/BoundInCode/AutoFileName): `文件路径自动提示` 
6. [gbk支持 GBK Encoding Support](https://github.com/akira-cn/sublime-gbk) 
7. [检测快捷键冲突](http://www.welefen.com/keymapmanager-add-check-plugins-keymap-conflict-feature.html) （没弄）
8. [markdown-preview](https://github.com/revolunet/sublimetext-markdown-preview)
9. [LineEndings 设置换行符](https://github.com/SublimeText/LineEndings) （没弄）
10. [html美化插件](https://github.com/rehorn/sublime-htmlbeautify) （没弄）
11. [Sublime Text 新建文件的模版插件: SublimeTmpl](http://www.fantxi.com/blog/archives/sublime-template-engine-sublimetmpl/) （没弄）
12. [前端自动化神器LiveReload配合浏览器和less/sass使用方法](http://www.cnblogs.com/liu-l/p/3902100.html) （没弄）
13. [全栈开发必备的10款 Sublime Text 插件 - 梦想天空（山边小溪） - 博客园](http://www.cnblogs.com/lhb25/p/10-essential-sublime-text-plugins.html)

    - [Git](https://packagecontrol.io/packages/Git)
    - [GitGutter](https://github.com/jisaacks/GitGutter)
    - [All Autocomplete](https://packagecontrol.io/packages/All%20Autocomplete) 
    - [Terminal](https://packagecontrol.io/packages/Terminal)—— `Ctrl / Cmd + Shift + T `，不过这也是打开上次关闭的文件的快捷方式，你需要修改一个快捷键来兼容两个功能 
    - [SublimeREPL](https://packagecontrol.io/packages/SublimeREPL)
    - [ColorPicker](https://packagecontrol.io/packages/ColorPicker)—— `Ctrl / Cmd + Shift + C `
14. [A File Icon](https://packagecontrol.io/packages/A%20File%20Icon)——展示文件图标
15. [FileDiffs](https://packagecontrol.io/packages/FileDiffs)——文件比较（强烈推荐）
16. [本地历史记录](https://github.com/vishr/local-history) （没弄）
17. [CSS值转REM的Sublime Text插件](https://github.com/flashlizi/cssrem) （没弄）
18. 其它语言框架支持 
    - [vue syntax highlight](https://packagecontrol.io/packages/Vue%20Syntax%20Highlight)
19. 版本管理
20. [CSScomb](https://packagecontrol.io/packages/CSScomb)——梳理CSS，即规范CSS属性书写顺序（强烈推荐） `C+S+c`
21. [SublimeCodeIntel](https://packagecontrol.io/packages/SublimeCodeIntel)——没有提示不能写demo了
22. [Tagify](https://packagecontrol.io/packages/Tagify)——为demo添加标签
23. [JsFormat](https://packagecontrol.io/packages/JsFormat)——格式化JavaScript代码
24. [SublimeTmpl](https://packagecontrol.io/packages/SublimeTmpl) ——快速生成文件模板 
25. [AdvancedNewFile](https://packagecontrol.io/packages/AdvancedNewFile)——快速创建新文件（C+A+n）
26. [FindKeyConflicts](https://packagecontrol.io/packages/FindKeyConflicts)——找快捷键冲突，直接使用 `C+S+p`输入Find什么的，老实说，英文的说明文档真不好懂，硬伤！

