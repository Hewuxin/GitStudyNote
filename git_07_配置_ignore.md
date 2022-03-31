##### 配置文件

- 项目配置文件 项目/.git/config

  ```
  git config --local user.name "Hewuxin"
  git config --local user.email "2386474352@qq.com"
  ```

- 全局配置文件: ~/gitconfig

  ```
  git config --global user.name "Hewuxin"
  git config --global user.email "2386474352@qq.com"
  ```
  
- 系统配置文件： /etc/.gitconfig  需要root权限

  ```
  git config --system user.name "Hewuxin"
  git config --system user.email "2386474352@qq.com"
  ```
- 应用场景

  ```
  git config --local user.name "Hewuxin"
  git config --local user.email "2386474352@qq.com"
  
  # 只是当前项目可以调用文件做冲突解决
  git config --local merge.tool bc3
  git config --local mergetool.path '/usr/local/bin/bcomp'
  git config --local mergetool.keepBackup false
  
  git remote add origin 地址  默认添加到本地配置文件中(--local)
  
  ```

##### git 免密登录

- URL中体现

  ```
  原来的地址： https://github.com/Hewuxin/dbhot.git
  修改的地址：https://用户名:密码@github.com/Hewuxin/dbhot.git
  git remote add origin https://用户名:密码@github.com/Hewuxin/dbhot.git
  git psuh origin dev
  ```

- SSh

  ```
  1. 生成公钥和私钥(默认放在~/.ssh)
     终端输入 ssh-keygen/ -r rsa
     id_rsa.pub 公钥
     id_rsa 私钥
  2. 拷贝公钥内容，并设置到github中
  3. 在git本地配置ssh地址
  	git remote add origin git@github.com:Hewuxin/dbhot.git
  4. 以后使用
  	git psuh origin master
  ```

- git自动管理凭证

##### ignore忽略文件

让Git不再管理当前目录下的某些文件。

```
在当前目录创建.gitignore文件
	a.h
	*.h  *指任意字符
	.gitignore
	files/ 忽略files文件夹下的所有文件
	
	*.h  指忽略所有的.h文件
	!a.h 指只管理a.h文件
```

github/gitignore中提供了每个语言的模板

规则

```
*.h
!a.h
files/
*.py[c|a|b] .pyc .pya .pyb 都忽略
```

##### git任务管理相关

- issues，文档以及任务管理
- wiki，项目文档。

