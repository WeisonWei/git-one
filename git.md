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
# 创建新项目后提交至远程仓库
## 1 在github上创建reactor3-core
## 2 在本地仓库提交并推至远程仓库
echo "# reactor3-core" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:WeisonWei/reactor3-core.git
git push -u origin master

```

```shell
# 将本地新项目代码提交至远程仓库
git remote add origin git@github.com:WeisonWei/reactor3-core.git
git push -u origin master
```


```shell
# 此命令会列出所有GIT当时能找到的配置
git config --list    
# 修改git提交的email
git config --global user.email test@test.com 
# 修改提交的git的user.name  
git config --global user.name test
```
