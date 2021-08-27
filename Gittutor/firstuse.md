# 初始设定
    git config --global user.name "<用户名>"
    git config --global user.email "<电子邮件>"
    git config --global color.ui auto

# 添加远程数据库
使用remote指令添加远程数据库。在\<name>处输入远程数据库名称，在\<url>处指定远程数据库的URL。
    
    git remote add <name> <url>
# 提交修改
## status
使用git status命令确认工作目录和缓存区的状态。

    git status
## 将文件加入缓存区
要使用add命令。在\<file>指定加入索引的文件。用空格分割可以指定多个文件。

    git add <file>..
> 指定参数「.」，可以把所有的文件加入到索引。

    git add .
## 使用commit提交
    git commit -m ""


## 使用push命令向数据库推送更改内容
\<repository>处输入目标地址，\<refspec>处指定推送的分支。我们将在高级篇详细地对分支进行说明。

    git push <repository> <refspec>
可以指定-u选项，那么下一次推送时就可以省略分支名称了

从克隆的数据库进行push时，使用

    git push
命令即可。