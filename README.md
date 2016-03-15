# 依赖项
 1. nodejs 5.2.0
 2. strongloop 6.0.0
 3. mysql Ver 14.14 Distrib 5.6.28, for Linux (x86_64) using  EditLine wrapper

# 安装环境

## mysql
1. wget http://dev.mysql.com/get/mysql-apt-config_0.3.5-1ubuntu12.04_all.deb
2. dpkg -i mysql-apt-config_0.3.5-1ubuntu12.04_all.deb
3. apt-get update
4. apt-get install mysql-server mysql-client
5. mysql_secure_installation

## nodejs
1. 下载nodejs编译包,wget https://nodejs.org/dist/v5.2.0/node-v5.2.0.tar.gz 
2. ./configure
3. make && make install

## 安装strongloop
1. npm -g install strongloop

## 安装forever
1. npm -g install forever

## 安装依赖项
1. cd build
2. npm install

# 启动命令
foever -l /log/access.log -e /log/error.log -o /log/out.log start . 