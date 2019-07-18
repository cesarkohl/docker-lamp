# Docker LAMP

PHP 7.2
MySQL 5.7

```
docker-compose up -d
docker ps
```

http://localhost

**Creating a user for MySQL**

```
docker-compose exec db bash
mysql -u root -p
root
show databases;
GRANT ALL ON db_test.* TO 'db_user'@'%' IDENTIFIED BY 'db_pass';
FLUSH PRIVILEGES;
EXIT;
exit
```

More info (code weren't working):

https://www.digitalocean.com/community/tutorials/how-to-set-up-laravel-nginx-and-mysql-with-docker-compose