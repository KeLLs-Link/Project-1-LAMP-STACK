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
































