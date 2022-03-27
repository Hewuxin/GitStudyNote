Beyond Compare

##### 快速解决冲突

1. 安装Beyond Compare

2. 在git中进行配置

   ```
   git config  --local merge.tool bc3  --local表示只在当前项目有效
   git config  --local mergetool.path 'Compare安装目录'
   git config  --local mergetool.keepBackup false  不用保留备份
   ```

3. 应用Beyond Compare 解决冲突

   ```
   git mergetool 
   ```

   