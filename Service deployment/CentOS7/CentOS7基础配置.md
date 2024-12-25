# CentOS7基础配置

### 





### 1.挂载本地源

```
[root@localhost ~]# rm -rf /etc/yum.repos.d/*
[root@localhost ~]# vim /etc/yum.repos.d/local.repo
[local]
name=local
baseurl=file:///mnt    #指定镜像挂载文件夹
enabled=1    #是否启用，1是启用
gpgcheck=0    #是否检测，0是不检查
[root@localhost ~]# mount /dev/sr0 /mnt    #将镜像挂载到本地
```

