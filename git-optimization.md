# Git 优化

在前两节中，我们安装完Git后，[创建并备份了公钥](https://gist.github.com/yisibl/8019693)，这篇教程让我们在使用 Git 时更加得心应手。

## 优化点

* 解决各种Git下的中文问题
* 显示中文文件夹或文件
* 显示中文git log信息
* 支持直接在bash输入中文
* 配置windows下的换行符问题
* 配置log，status等命令自动颜色高亮
* 全局的.gitignore配置，不必在每个仓库下手动配置.gitignore文件了
* 设置常用命令缩写
    git co = git checkout
    git br = git branch
    git ci = git commit
    git st = git status
    git dt = git difftool
    git mt = git mergetool
* 设置commit信息编辑器，windows下使用notepad2，其它系统使用Vim
* 设置代码合并工具，windows下使用TortoiseMerge，其它系统使用VimDiff
* 添加Git命令按Tab键自动补全功能（Linux）
* 更多等待你发现…

## 安装方法

* 下载最新的 [优化包](http://gitlab.alibaba-inc.com/qiyao.kxp/gitconfig/tree/master)     
* 访问密码 `7HCOpF`

### Windows

1. 下载[优化包](http://www.kuaipan.cn/file/id_214486852831281154.htm)
1. 解压缩文件，进入gitconfig目录，将里面的文件全部复制到Git安装目录下的cmd文件夹中
1. 启动一个Git Bash窗口
1. 执行命令(一丝和yiorsi@gmail.com为可选参数，使用时替换成你自己的信息)

```git
gitconfig init 一丝 yiorsi@gmail.com
```

> 如果执行gitconfig的时候报错，并提示“找不到这个命令”，说明在安装git的时候没有把安装路径加入到path中，这时候只需要把git安装目录下的cmd目录路径添加到path环境变量中就可以了。  
在Git Bash无法输入中文怎么办？
* 先不带参数执行一次“gitconfig init”。重新打开Git Bash，现在可以输入中文了！再加上参数执行一次呗！
* Git V1.7.10 开始引入了 Unicode 支持，所以在此版本之前会出现的乱码问题可能在之后的版本则不需要设置，但仍存在一些乱码问题。

### Linux & Mac

1. 新建文件夹

```
mkdir gitconfig  
cd gitconfig
```
2. 下载压缩包

```
curl -O http://ux.etao.net/git/gitconfig/gitconfig.tar.gz
```
3. 解压缩，添加可执行权限

```
tar zxvf gitconfig.tar.gz  
chmod +x gitconfig git_config_init git_config_update
```
4. 执行配置脚本(一丝和yiorsi@gmail.com为可选参数，使用时替换成你自己的信息)

```
./gitconfig init 一丝 yiorsi@gmail.com
```

## 升级方法

version 0.0.2版本开始支持在线升级

### Windows

启动一个Git Bash窗口，执行下面的命令

```
gitconfig update
```
### Linux
进入您的gitconfig目录，执行下面的命令

```
./gitconfig update
```


## 命令介绍

* 初始化gitconfig配置信息
    ```
    gitconfig init
    ```


* 在线升级你的gitconfig，0.0.2版本开始支持
    ```
    gitconfig update
    ```


**Windows下在线升级需要管理员权限，请使用管理员身份运行Git Bash**

## 更多

* [msysGit 中文环境配置及跨平台开发注意事项](http://baifa.me/2010/10/msysgit.html)
* [惊艳的cygwin——Windows下的Linux命令行环境的配置和使用](http://oldratlee.com/post/2012-12-22/stunning-cygwin)