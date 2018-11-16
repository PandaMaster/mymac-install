# mymac-install
Mac上有一部分软件需要通过命令行的进行安装和更新。一般的命令都比较长，不容易记住。在这里记录下命令的使用手顺，方便再次使用时查找。

## 目录
* [VIM](#VIM)
* [Homebrew](#Homebrew)
* [Python](#Python)

## VIM
MAC系统(10.11.6)自带VIM的版本是7.3，有很多插件都使用不了。  
可以通过安装MacVim将VIM的版本升级到7.4。  
直接在命令行输入`vim`就可以看到vim的版本。  
安装MacVim的命令:`brew install macvim --with-lua --with-override-system-vim`  
MacVim实际上就是有图形界面的VIM，操作方式和VIM类似。  
可以通过Alfred的快捷键直接打开MacVim，但是Spotlight却搜索不到。

## Homebrew
[Homebrew](https://brew.sh/)是一款MacOS平台下的软件包管理工具，拥有安装、卸载、更新、查看、搜索等很多实用的功能。  
- 安装  
`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
- 更新
`brew update`
由于国内GFW的原因，直接更新会没有响应。需要替换更新源[清华大学镜像](https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/)。
```
cd "$(brew --repo)"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git

cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git

brew update
```

## Python
1.使用homebrew搜索python  
`brew search python`  
2.安装python  
`brew install python3`
