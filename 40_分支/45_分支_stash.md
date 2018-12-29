
# 1 概述

    在修复紧急bug的时候,
    当前的修改存起来,清空工作区和暂存区
    切一个新的分支,去修复bug
    修复完成以后,将存起来的修改释放回原先分支的区域


# 2 stash

命令 

    git stash <save name>
    
效果 

    可以把对当前分支的修改(工作区/暂存区)隐藏到当前分支的仓库中

示例
```
$ git stash
Saved working directory and index state WIP on dev: 6224937 add merge
HEAD is now at 6224937 add merge

查看修改
git status查看工作区，就是干净的
```

# 3 显示隐藏列表

命令 
    
    $ git stash list
    
    
效果
  
    stash@{0}: WIP on dev: 6224937 add merge

# 4 恢复隐藏数据

命令 
    
    git stash apply stash{}

示例

    $ git stash apply stash@{0}
    恢复后，stash内容并不删除，你需要用git stash drop来删除；

