# Git常用命令

```shell
— 1 代码操作
— 1.1 克隆代码
git clone *******.git
— 1.2 更新代码
git pull
```

```shell
— 2 提交代码三步骤
- 2.1 查看状态
git status -s
- 2.2 提交到本地仓库并添加注释
git commit -am "modify test case"
- 2.3 提交至远程仓库
git push
```
```shell
— 3 分支操作
— 3.1 创建分支
git branch branchName
— 3.2 删除远程仓库分支
git push origin --delete branchName
— 3.3 删除本地仓库分支
git branch -d branchName
— 3.4 查看所有分支
git branch -a
— 3.5 切换分支
git checkout evan
— 3.6 将当前代码提交到一个新分支上（即:以当前代码创建新分支）
git push origin branchOld:branchNew
— 3.7 下载指定分支
git clone xxxxxxxxxxxxx.git -b branchName
```


```shell
# 此命令会列出所有GIT当时能找到的配置
git config --list    
# 修改git提交的email
git config --global user.email test@test.com 
# 修改提交的git的user.name  
git config --global user.name test
```

```shell
# 往github上提交刚创建的新项目
# create a new repository on the command line
echo "# mysql-jdbc" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M trunk
git remote add origin https://github.com/WeisonWei/mysql-jdbc.git
#初次关联远程仓库以后用 将会关联到远程的master 分支上，以后就可以git push不指定参数了
git push -u origin trunk
```

```shell
# push an existing repository from the command line
git remote add origin https://github.com/WeisonWei/mysql-jdbc.git
git branch -M trunk
git push -u origin trunk
```