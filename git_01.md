##### git安装

官网安装 安装成功之后通过 git --version查看

##### git 生成版本

git init 初始化仓库

git status 检测当前文件夹下边的文件状态

git add  .  点代表当前文件夹未被管理的所有文件

git commit -m "描述信息"

- git commit -m "第一个版本"

- git status

  - ```
    On branch master
    nothing to commit, working tree clean
    意味着当前文件夹里的所有文件都被git管理起来，生成了一个版本
    ```

  - ```
      modified:   git_01.md
    说明在上一个版本的基础上修改了 git_01.md文件
    ```

git add . 再一次 管理修改的文件