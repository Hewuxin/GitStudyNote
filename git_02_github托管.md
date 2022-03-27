#### github/gitlab

##### 注册账号

#####  创建仓库

##### 本地代码推送到远程仓库

1. 本地没有代码

   ```
   首先创建 README.md
   git init 
   git add README.md
   git commit -m "first commit"
   git remote add origin https://github.com/heyuyang/git_note.git 给远端仓库起别名
   git push -u origin 分支  向远程推送代码
   ```

2. 本地有代码

   ```
   git remote add origin https://github.com/heyuyang/git_not.git
   git push -u origin master 推送到远端master分支
   ```

##### 将远程仓库代码克隆到本地

```
git clone 远程仓库地址 （内部已经实现了git remote add origin 远程仓库 这一操作）
git log
git status
git branch  虽然只显示一个master分支 但其实master 和dev分支都copy了 
git checkout dev 可以直接切换到dev分支
```



