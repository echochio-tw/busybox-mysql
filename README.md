# busybox-mysql

git it and biuld it
```
git clone https://github.com/echochio-tw/busybox-mysql
cd busybox-mysql
docker build -t mysql-busybox .
```

run it
```
docker run -d -p 192.168.0.70:3306:3306 --name=mysql-busybox mysql-busybox
```

check it
```
# mysql -h 192.168.0.70 -u root -prootpass
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MySQL connection id is 3
Server version: 5.7.16 MySQL Community Server (GPL)

Copyright (c) 2000, 2016, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MySQL [(none)]>
```

openshift docker use it

pull from docker ......
docker.io/echochio/mysql

![alt tag](https://github.com/echochio-tw/busybox-mysql/raw/master/show.png)


