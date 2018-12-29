


# 1 概述

    使用git_flow管理开发中的问题


# 2 分支说明

master 

    作用  发布版本 (发布阶段)
    
    流程  接受Release和Hotfix分支
         所有在Master分支上的Commit应该Tag
    
Develop

    作用  开发主分支 (开发阶段)
    流程  从master分支创建, 接受Feature和Hotfix的合并,目的是创建Release分支    

Feature 

    作用    细分业务功能分支(开发阶段)
    分支名  feature-pay1
    流程    从develop创建Feature分支,功能做完后，合并回Develop分支


Release

    作用      整体版本功能(开发完成,进入测试) 
    分支名     release-pay
    流程  
            Release分支基于Develop分支创建，打完Release分之后，我们可以在这个Release分支上测试，修改Bug等。
            同时，其它开发人员可以基于开发新的Feature (记住：一旦打了Release分支之后不要从Develop分支上合并新的改动到Release分支)
            发布Release分支时，合并Release到Master和Develop， 同时在Master分支上打个Tag记住Release版本号，然后可以删除Release分支了。    

Hotfix

    作用      修复紧急bug (运维阶段)
    分支名     hotfix-paybug
    流程      hotfix分支基于Master分支创建，
             开发并测试完后需要合并回Master和Develop分支，




# 3 工作流程


# 4 特别说明


## 4.1 提交

    每次的提交最好都保存在远程,比较安全
    多次提交保存为一次提交

## 4.2 合并
    
    为了记录分支的完整活动
    使用 merge不使用rebase
    使用 merge --no-ff
    
release 合并 到 master

        


# 5 参考

[git-flow](https://www.cnblogs.com/cnblogsfans/p/5075073.html)