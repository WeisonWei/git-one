# Git Submodule 用法

## 新增submodule
```$xslt
git submodule add git://github.com/majutsushi/tagbar.git .vim/bundle/tagbar
```
## 更新submodule
個別repo更新比較麻煩,必須到個別的目錄底下執行git pull去拉upstream的程式碼,可是這樣會比較安全；
若要一次全部更新所有的submodule可以用這foreach指令:
```$xslt
git submodule foreach --recursive git pull origin master
```
## 刪除submodule

    1 使原先子模块不被版本控制（先把子模块从版本控制系统移除）`git rm --cached /path/to/files`
    2 删除子模块目录`rm -rf /path/to/files`
    3 修改.gitmodules,移除这个submodule
    4 修改.git/config内容,把需要删除的submodule配置项删除  -- 执行commit
    5 修改.git/modules文件夹内容,把你想要删除的子模块目录删除


[参考](https://blog.chh.tw/posts/git-submodule/)