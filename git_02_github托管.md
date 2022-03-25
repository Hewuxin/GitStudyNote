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
   git push -u origin master
   ```

2. 本地有代码

   ```
   git remote add origin https://github.com/heyuyang/git_not.git
   git push -u origin master 推送到远端master分支
   ```

   

