

# 概述 (推荐使用)

优点
    0.可视化管理git
    1.为原生的GIT操作
    2.版本和分支管理更清晰
    3.能够完成几乎所有的功能
    
缺点

    代码冲突没有IDEA直观
    合并时,使用了fast forwad


# 安装

## 下载

    https://www.sourcetreeapp.com
    或者百度云

## 安装

    一路next就行

### 登录注册问题


1.翻墙注册
    如果遇到Cannot load JavaScript的问题,可以尝试下面的方法
2.免注册
```
1.进入C:\Users\你的电脑名字\AppData\Local\Atlassian\SourceTree 
2.添加accounts.json
    内容
    [  
      {  
        "$id": "1",  
        "$type": "SourceTree.Api.Host.Identity.Model.IdentityAccount, SourceTree.Api.Host.Identity",  
        "Authenticate": true,  
        "HostInstance": {  
          "$id": "2",  
          "$type": "SourceTree.Host.Atlassianaccount.AtlassianAccountInstance, SourceTree.Host.AtlassianAccount",  
          "Host": {  
            "$id": "3",  
            "$type": "SourceTree.Host.Atlassianaccount.AtlassianAccountHost, SourceTree.Host.AtlassianAccount",  
            "Id": "atlassian account"  
          },  
          "BaseUrl": "https://id.atlassian.com/"  
        },  
        "Credentials": {  
          "$id": "4",  
          "$type": "SourceTree.Model.BasicAuthCredentials, SourceTree.Api.Account",  
          "Username": "",  
          "Email": null  
        },  
        "IsDefault": false  
      }  
    ]  
3.重新启动安装文件,并选择我不想使用Mercural

4.参考 
只需要这一次登陆就行,以后都不用了
http://blog.csdn.net/jiangyu1013/article/details/78850735   
```


# mac安装

使用SourceTree Mac版免登录版
地址




# git flow 操作

