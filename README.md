## 背景

该项目存储mysql相关问题及配置

## 配置文件my.cnf

5.7.18后mysql不再提供默认的my.cnf配置文件, 为此该项目提供其模板样例文件

使用命令`mysql --help|grep my.cnf`可知, mysql读取配置文件的路径顺序依次为: 

* /etc/my.cnf
* /etc/mysql/my.cnf
* /usr/local/mysql/etc/my.cnf
* /usr/local/mysql/my.cnf
* ~/.my.cnf 

所以将文件`my.conf`拷贝至 `/etc/my.cnf`目录下, 重启mysql即可.

## mysql相关指令

* 状态: `usr/local/mysql/support-files/mysql.server status`
* 启动: `usr/local/mysql/support-files/mysql.server start`
* 停止: `usr/local/mysql/support-files/mysql.server stop`
* 重启: `usr/local/mysql/support-files/mysql.server restart`
