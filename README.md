# GitCommonCommand
git common command

1.克隆远程分支:
```objc
$ git clone url -b branch_name /your/folder
例: $ git clone https://github.com/fengyueran/Test.git -b dev
```

2.查看当前配置有哪些远程仓库:
```objc
$ git remote
例: $ git remote –v  显示对应的克隆地址
```

3.推送到远程分支:
```objc
$ git push <remote-name> <branch-name>
例: $ git push origin dev/IOS-Design-Patterns
```

4.git配置用户密码
```objc
$ git 
```

5.新建分支
```objc
$ git branch <branchname>
例: $ git branch dev/app
```

6.切换分支
```objc
$ git checkout <branchname>
例: $ git checkout dev/app
```

7.新建并切换分支
```objc
$ git checkout -b <branchname>
例: $ git checkout -b dev/app
```

8.删除分支
```objc
$ git branch -d <branchname>
例: $ git branch -D dev/app(D强制删除)
例: $ git push origin --delete dev/CoreData(删除远程分支)
```

9.查看配置信息
```objc
$ git config –list
```

10.删除全局配置文件的用户名和邮箱
```objc
$ git config --unset --global user.name "fengyueran"
$ git config --unset --global user.email 316032603@qq.com
```

11.git 如何让单个文件回退到指定的版本
```objc
1).进入到文件所在文件目录，或者能找到文件的路径
$ git reflog MainActivity.js
2) 回退到指定的版本$  git reset ecb2cae MainActivity.js
3) 可用sourceTree右键回退。
```

12.合并分支
```objc
$ git rebase master（将master分支合并到当前分支)
$ git merge hotfix（将hotfix分支合并到当前分支）
```

13.解决冲突
```objc
$ git mergetool -t kdiff3
```

14.合并提交历史
```objc
$ git merge --squash hotfix
```

15.追加到上一次提交
```objc
$ git commit --amend
```

16.查看某个命令的帮助
```objc
$ git commit –help
```

17.添加远程仓库
```objc
$ git remote add pb git://github.com/paulboone/ticgit.git
```