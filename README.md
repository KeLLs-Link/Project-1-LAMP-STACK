# WEB STACK IMPLEMENTATION (LAMP STACK) IN AWS
___

### Ubuntu Linux VM EC2 Instance succefully pinned up on AWS Cloud
![Screenshot (206)](https://user-images.githubusercontent.com/57721371/204056046-527798a6-eefe-4f41-ae7e-14bb468a649b.png)

``` 
ssh -i "newkeypair.pem" ubuntu@ec2-34-224-93-250.compute-1.amazonaws.com
```
___

### Apache Web Server installed using Ubuntu's Package Manager "apt"
![Screenshot (210)](https://user-images.githubusercontent.com/57721371/204056522-a9e2c2e7-2a52-4f12-855a-b81f0bc2b87a.png)
```
Run apache2 package installation
sudo apt install apache2
```
___

### Apache default web page view on a web browser using EC2 public IP addres
![Screenshot (212)](https://user-images.githubusercontent.com/57721371/204057261-d3d4fcbb-5a49-4667-8ea8-cf2f8f6b080d.png)
```
curl http://34.224.93.250:80
```
___
### MySQL Database Management System succesfully installed.
![Screenshot (213)](https://user-images.githubusercontent.com/57721371/204059014-06fb2736-73f2-4d05-9f4c-1613203b4e21.png)
```
sudo apt install mysql-server
```
___
### Succesfully logged into MySQL Database
![Screenshot (214)](https://user-images.githubusercontent.com/57721371/204059490-3598686e-a14a-4b2c-a2ba-37f3f0490769.png)
```
sudo mysql
```
___
### Root user password set using root user MySQL_native_password; PassWord.1
![Screenshot (215)](https://user-images.githubusercontent.com/57721371/204060023-8788305e-0e0f-4899-85b0-c5bc1fe08835.png)
```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';
```
___
### All three Php packages viz: php-mysql, libapache2-mod-php, php core packages automatically installed as dependencies
![Screenshot (216)](https://user-images.githubusercontent.com/57721371/204061851-a56b1992-59cf-4a17-bbf8-0affd7245976.png)
```
sudo apt install php libapache2-mod-php php-mysql
```
___
### Myfirstlampproject directory created and ownership assigned 
![Screenshot (218)](https://user-images.githubusercontent.com/57721371/204062216-cb9c9aee-bea2-4cfe-a3ec-cbca98e0ed74.png)
```
sudo mkdir /var/www/projectlamp
sudo chown -R $USER:$USER /var/www/projectlamp
```
___
### A new configuration file was created using vim (Vi-Improved)- an open source screen based text editor
![Screenshot (220)](https://user-images.githubusercontent.com/57721371/204062568-b40cb731-2d57-46e7-a380-095ffa84f80e.png)
```
sudo vi /etc/apache2/sites-available/projectlamp.conf
```
___
### Enabling php content on the website 
![Screenshot (223)](https://user-images.githubusercontent.com/57721371/204062758-90043c63-44c1-4204-af2d-15d1fb2a4229.png)
```
sudo vim /etc/apache2/mods-enabled/dir.conf

<IfModule mod_dir.c>

#Change this:

#DirectoryIndex index.html index.cgi index.pl index.php index.xhtml index.htm

#To this:

DirectoryIndex index.php index.html index.cgi index.pl index.xhtml index.htm

</IfModule>
```
___
### creating an index.php file inside a custom web root folder
![Screenshot (230)](https://user-images.githubusercontent.com/57721371/204062967-41265322-233b-4659-9603-b6f87eab8013.png)

```
vim /var/www/projectlamp/index.php
<?php

phpinfo();
```































