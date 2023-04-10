本讲的内容主要是关于`git log`命令更细致的用法

# 1.git commit -m'' 和 git commit -am'' 有什么区别
`git commit -m 'message'` 和 `git commit -am 'message'` 命令的区别在于：

* `git commit -m 'message'` 只会将已经跟踪的文件中的变更提交到本地仓库，并附带一条简短的提交信息。
* `git commit -am 'message'` 除了将已经跟踪的文件中的变更提交到本地仓库之外，还会自动将所有未被 Git 忽略的文件添加到暂存区中。

需要注意的是，`git commit -am 'message'` 只会将之前已经被 Git 跟踪的文件添加到暂存区中。如果你新建了一个文件并且希望将它添加到暂存区中，你需要使用 `git add` 命令来完成此操作。

# 2. git log 的几个操作
* git log --all 展示所有变更历史，包括所有分支
* git log -n3   展示最近三条的变更历史
* git log --oneline 每一条变更都在同一行展示
* git log --graph 以图形界面的方式展示(虽然我觉得没啥用)
