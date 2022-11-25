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




















