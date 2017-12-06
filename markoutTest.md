#Git操作笔记
###创建版本库
什么是版本库呢？版本库又名仓库，英文名repository，你可以简单理解成一个目录，这个目录里面的所有文件都可以被Git管理起来，**每个文件的修改、删除**，Git都能跟踪，以便任何时刻都可以追踪历史，或者在将来某个时刻可以“还原”。
- 创建一个learngit文件准备作为git仓库
```
$ mkdir learngit
$ cd learngit
$ pwd
//pwd命令用于显示当前目录
```
- 将该文件夹初始化为git仓库
``` 
$ git init
```
- 添加文件进入learngit仓库
1. 将本地文件拖进该仓库文件夹
2. 
``` 
$ git add readme.txt
//将该文件添加进仓库(注意：可以反复添加，再一次性commit)
```
3.//用命令git commit告诉Git，把文件提交到仓库：
```
 $ git commit -m "wrote a readme file"
//-m后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录。
```
4. 补充&小结：
- **cat** 文件名 可以读取文档内容
- git status命令可以让我们时刻掌握仓库当前的状态
- git diff顾名思义就是查看difference，在后面添加文件名字后就可以看到具体修改了什么，确认修改内容后就可以commit文件了。
- 要随时掌握工作区的状态，使用git status命令。
- 如果git status告诉你有文件被修改过，用git diff可以查看修改内容。