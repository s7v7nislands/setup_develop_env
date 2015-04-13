#配置步骤

根据下面生成开发环境

##软件列表

需要安装一下软件:

1.	[virtualbox](https://www.virtualbox.org)
2.	[vagrant](https://www.vagrantup.com)
3.	[packer](https://packer.io)
4.	[docker](https://www.docker.com)

##安装步骤

1.	安装virtualbox
2.	安装vagrant

###生成虚拟机

```shell
mkdir debian
cd debian

vagrant init chef/debian-7.8
vagrant up
vagrant ssh
```

这个时候已经运行在debian中,已经拥有所有权限.

###更新系统

```shell
apt-get update
apt-get upgrade
```

###安装python运行环境

```shell
apt-get install virtualenv pip
```

### virtualenv创建独立的python开发环境

```shell
virtualenv dev
cd dev
source bin/activate
```
