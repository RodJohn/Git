
# GitLab 

    GitHub中存储私有项目要收费。
    GitLab 则是开源免费，同样是采用了 Ruby on Rails 开发，可以自己搭建GitHub

## 参考

https://www.gitlab.cc/

# 安装

## 硬件要求
	gitlab项目中包含了大量的服务(如redis.postgre)需要大量的硬件资源,推荐生产环境中使用4G内存，2核CPU。官方参考文档https://docs.gitlab.com/ce/install/requirements.html
	第一次启动的时候，需要初始化大量的东西，经常会出现502错误，通常是由于内存不足的原因导致。

## 安装

### yum

配置国内yum源
https://mirror.tuna.tsinghua.edu.cn/help/gitlab-ce/


## 配置

### 配置gitlab.rb

vim  /etc/gitlab/gitlab.rb
把external_url后面的值改成部署机器的域名或者IP地址和端口
默认是8080端口
如 external_url 'http://39.108.224.136:9000'
这个地址很重要，上传的图片什么的，url会以这个为基准，如果地址写错，将无法访问到图片等这些资源。

### 重置

gitlab-ctl reconfigure


## 启动GitLab

gitlab-ctl restart

启动成功
```
ok: run: gitlab-git-http-server: (pid 3922) 1s
ok: run: logrotate: (pid 3929) 0s
ok: run: nginx: (pid 3936) 1s
ok: run: postgresql: (pid 3941) 0s
ok: run: redis: (pid 3950) 0s
ok: run: sidekiq: (pid 3955) 0s
ok: run: unicorn: (pid 3961) 1s
```


## 登陆
访问external_url中配置的url及相应端口
第一次会要求为gitlab账号root设置密码(gitlab123)


# 常用命令

gitlab-ctl stop



# 其他考虑

发消息
http://www.jianshu.com/p/a22eaa1fcfe7