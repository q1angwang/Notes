

git add -A
git add --all
它能stages所有文件，而之前用的

git add .
只能stages新文件和被修改文件，没有被删除文件

建议每一次add之后再次使用git status命令来查看是否已经stage了







$ git status
On branch master
Your branch and 'origin/master' have diverged,
and have 22 and 23 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean

WQ@DESKTOP-3BGM28T MINGW64 ~/Documents/CloudFile/Work/Notes/2019Course (master)
$ git merge origin/master
fatal: refusing to me


git merge master --allow-unrelated-histories









Your branch and 'origin/master' have diverged, and have 1 and 1 different commits each, respectively
2017年12月26日 14:10:28 Lframe 阅读数：5471
当我们在本地提交到远程仓库的时候，如果遇到上述问题，我们可以首先使用如下命令：

git rebase origin/master 

然后使用

git pull --rebase 

最后使用

git push origin master 

把内容提交到远程仓库上