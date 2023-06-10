---
title: Git-Basic 1
date: 2023-06-10 15:35:49
tags:
---

## Git 常用命令-1

### 配置

 ``` shell
 git config --global user.name "[name]"
 ```

设置在所有仓库中使用的用户名。[name]应替换为你选择的名字。

``` shell
git config --global user.email "[email address]"
```

设置在所有仓库中使用的邮箱地址。[email address]应替换为你选择的邮箱地址。

### 创建和克隆仓库

``` shell
git init [repository name]
```

创建一个新的本地仓库，名字是[repository name]。

``` shell
git clone [url]
```

从URL下载项目和其完整的版本历史。

### 提交

``` shell
git status
```

查看你的仓库当前的状态。

``` shell
git add [file]
```

将文件添加到暂存区。

``` shell
git commit -m "[descriptive message]"
```

提交你的改动，并附带一条说明你所做改动的信息。

### 分支

``` shell
git branch
```

列出本地存在的所有分支。

``` shell
git branch [branch name]
```

创建一个新分支，名字是[branch name]。

``` shell
git checkout [branch name]
```

切换到名为[branch name]的分支。

``` shell
git merge [branch]
```

合并指定分支到当前分支。

### 远程仓库操作

``` shell
git push [alias] [branch]
```

将分支推送到远程仓库。一般alias用**origin**，branch为**main**

``` shell
git pull
```

获取并合并远程仓库的最新更改。

### 历史

``` shell
git log
```

查看提交历史。

``` shell
git log --summary
```

查看更详细的提交历史。

``` shell
git log --oneline
```

查看一行的提交历史。

### 撤销

``` shell
git reset [commit]
```

撤销所有[commit]后的提交，保留改动。

``` shell
git reset --hard [commit]
```

撤销所有[commit]后的提交，丢弃改动。
