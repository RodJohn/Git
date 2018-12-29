# intellij IDEA


## 设置git

    界面进入setting>git 
    填入git安装地址
    选择native方式执行

## 常用操作

	git add  
			新建文件的时候会提示是否加入
			或者右键文件选择git--add
	git status
			点击Version Control 视图-->local Change
			可以看到加入版本控制,和未加入版本控制的文件
	git check -- 
			右键文件选择git--revert
			将文件移除版本控制
	查看文件改变
			右键文件-->SHOW diff
			
	git pull
			点击右上角 updateProject图标
			最好先将代码提交完整
			选择merge+stash 
			    stash是git原生的代码搁置。shelve是idea独有的
			    merge保存操作历史,rebase不保存
	如果有冲突
			直接在中间修改,并选择Apply
	
	git commit/push
			点击右上角 commit 图标
			同时可以推到远程仓库
			
    
     

## 其他

	其他操作可以右键文件选择git
	或者VCS-->GIT


### 问题 Could not read from remote repository

    1.替换失效公钥
    2.将idea的git插件选择native方式执行