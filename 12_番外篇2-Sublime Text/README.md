#小课堂番外篇2-工具之Sublime Text 3
Sublime Text是一个文本编辑器，比较易于使用（相比其他繁复的IDE等等来说，所以我们可以暂时用它来作编辑器，以后大家想换也是可以哒……而且很好看QwQ）
##安装
[Sublime Text 3下载地址](http://www.sublimetext.com/3)

选择你的系统对应的版本，下载安装。

没有之前那么痛苦啦，它就正常的装完了，有一个勾选的地方，勾了就好，意思是加到菜单里这样右键就能用sublime打开文件了。

OS X的话装好把它拖到application里；

Windows如果木有建快捷方式就建个快捷方式或者固定到任务栏。
##优化
介绍戳[这里](https://packagecontrol.io/installation)，可以尝试自己看看。

Package Control是Sublime的插件管理器，可以方便Sublime的插件管理，这样我们就可以安装各种插件来辅助编程啦。
###安装
然后simple的安装方法是这样滴：

打开sublime，用快捷键`ctrl+C`或者从菜单的`View-Show Console`打开console，在下方小窗复制粘贴下面的代码然后回车，就会开始下载package control。
```
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```
下载需要花费一些时间，会卡一会儿。可能会跳出提示窗口，确定就好。

然后安装完了，重启Sublime。
###使用
快捷键`crtl+shift+P`或者菜单`Tools-Command Paletter`跳出一个窗口，输入`install`，选中`Install Package`并回车，会开始加载插件列表。

这个时候编辑器窗口的左下角会有动画（一个跑来跑去的`=`符号），说明在加载插件列表，但是由于墙的原因，可能非常非常慢……或者根本加载不出来。恩加载不出来也不要灰心……翻墙后篇再说。

如果加载出了插件列表，在里面查找自己需要的插件，就可以下载安装。

##额外提醒
###Special for Mac
Anytime，如果弹出提示xcrun要求安装命令行工具，请点击安装。
