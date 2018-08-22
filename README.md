# mymac-install
Mac上有一部分软件需要通过命令行的进行安装和更新。一般的命令都比较长，不容易记住。在这里记录下命令的使用手顺，方便再次使用时查找。

## 目录
* [VIM](#VIM)
* [Python](#Python)

## VIM
MAC系统(10.11.6)自带VIM的版本是7.3，有很多插件都使用不了。  
可以通过安装MacVim将VIM的版本升级到7.4。  
直接在命令行输入`vim`就可以看到vim的版本。  
安装MacVim的命令:`brew install macvim --with-lua --with-override-system-vim`  
MacVim实际上就是有图形界面的VIM，操作方式和VIM类似。  
可以通过Alfred的快捷键直接打开MacVim，但是Spotlight却搜索不到。

## Python
1.使用homebrew搜索python  
    brew search python  
2.安装python  
    brew install python3
