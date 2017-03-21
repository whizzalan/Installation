
```shell
#### CentOS 6.8 / HDP 2.4.2.0 ####

## install httpd ##
yum install httpd
service httpd start
vim /etc/httpd/conf/httpd.conf
# ServerName <IP>:80

cd /var/www/html
mkdir ambari
cd /var/www/html/ambari
# wget http://public-repo-1.hortonworks.com/ambari/centos6/2.x/updates/2.2.2.0/ambari-2.2.2.0-centos6.tar.gz
tar -zxvf ambari-2.2.2.0-centos6.tar.gz

## check httpd
service httpd restart

## using lynx check 
yum install lynx # default base repo
lynx http://<hostname>/ambari
```



