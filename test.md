### git与github的关系

git是一个版本管理工具（软件工具）；github是用git做版本控制的项目托管平台（一个网站）。

### 在windows上如何安装Git？
   **msysgit**是 windows版的Git,如下：
![](http://ww1.sinaimg.cn/mw690/6941baebgw1eloyr9g0xxj206u00tt8j.jpg)

#### 最新版本下载地址
[下载地址](https://git-for-windows.github.io/)

### 注册github账号
官方网址：[https://github.com/](https://github.com/)
![](http://img.blog.csdn.net/20161215154849180?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvZmVuZ3Fpbmd0YW8yMDA4/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

注册界面   sign up 是注册，sign in 是登录
![](http://img.blog.csdn.net/20161219155249954?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvZmVuZ3Fpbmd0YW8yMDA4/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### 了解一些简单系统命令

#### pwd 
获得当前所在目录

#### mkdir
创建目录命令：格式如下

> mkdir 新建的目录名
#### cd命令
进入到某个目录
> cd 目录名

举例子,进入到d盘hello目录
```
cd d:/hello
```
### 了解常用git命令

1. git初始化

```
git init
```
该命令执行后会出现一个.git的隐藏文件夹，这个文件里的内容是：

![image.png](http://upload-images.jianshu.io/upload_images/468490-cb8cde49aef4c341.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这里面的内容，会保存我们对整个**项目**的所有修改的记录，可以使得我们恢复到之前的任何状态。

2. git add 把工作区的文件提交到暂存区

git add 文件名
git add . （添加目录里所有文件）

![](http://upload-images.jianshu.io/upload_images/1132519-c1ba4dea31c7c001.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/700)
3. git commit 把工作区的文件提交到本地仓库Repository
git commit -m"本次提交的描述"

第一次运行git commit命令会出现以下提示：

![image.png](http://upload-images.jianshu.io/upload_images/468490-93d59782d2d28745.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

解决办法：
 1.设置用户名
```
    git config --global user.name "zhangsan"
```
  2.设置用户名邮箱
```    
git config --global user.email  "zhangsan@sina.com"
```

### 本地仓库操作总结

新建一个项目以后，首先调用一次git init命令初始化一个仓库。接下随着新文件的增加和修改，不断 的调用git add . 和git commit -m"xxx"命令，将整个开发的过程保存到仓库中。

> 到此为止和github还没有任何关系。

### 把本地仓库的内容上传到github

1. 登录github后，在github新建一个对应的仓库（保存我们的项目）

2.运行以下命令 ：
git remote add 远程项目别名 远程项目地址
```
git remote add origin git@github.com:songboriceboy/my_novel_project.git
```
3. 将本地仓库上传远程仓库（github上自己用户的新建项目中）

git push -u 远程地址 本地仓库（默认叫master）

```
git push -u origin master
```
一般需要输入用户名和密码：可能如下图所示：
![image.png](http://upload-images.jianshu.io/upload_images/468490-7ef3aa80e6df7aae.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这时，我们需要将自己的电脑，在github上添加为被信任。

创建SSH Key。在用户主目录下，看看有没有.ssh目录，如果有，再看看这个目录下有没有id_rsa和id_rsa.pub这两个文件，如果有的话，直接跳过此如下命令，如果没有的话，打开命令行，输入如下命令：

ssh-keygen  -t rsa –C "zhangsan@sohu.com"