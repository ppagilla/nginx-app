#INSTALLING WEBSERVER apache2/nginx: 

Installing apache2/httpd on AmazonMachine Linux image: (working)

#!/bin/bash
sudo yum update -y
sudo yum install httpd git php -y
sudo rm -rf /var/www/html/*
sudo git clone https://github.com/ppagilla/nginx-app.git /var/www/html/
sudo systemctl start httpd



Installing nginx on AmazonMachine Linux image: (working)

#!/bin/bash
sudo yum update -y
sudo yum install nginx php git -y
sudo rm -rf /usr/share/nginx/html/*
sudo git clone https://github.com/ppagilla/nginx-app.git /usr/share/nginx/html/
sudo systemctl start nginx


====================

Installing apache2/httpd on ubuntu Linux image:  (working)

#!/bin/bash
sudo apt update -y
sudo apt install apache2 git php -y
sudo rm -rf /var/www/html/*
sudo git clone https://github.com/ppagilla/nginx-app.git /var/www/html/
sudo systemctl start apache2



Installing nginx on ubuntu Linux image: (Not working)

#!/bin/bash
sudo apt update -y
sudo apt install nginx php git -y
sudo rm -rf /usr/share/nginx/html/*
sudo git clone https://github.com/ppagilla/nginx-app.git /usr/share/nginx/html/
sudo systemctl start nginx

same as above (Not working):

#!/bin/bash
sudo apt update -y
sudo apt install nginx php git -y
sudo rm -rf /usr/share/nginx/html/*
sudo git clone https://github.com/ppagilla/nginx-app.git /usr/share/nginx/html/
sudo systemctl start nginx

echo "hai" > /tmp/pavan.txt
ls /var/www/html/ >> /tmp/pavan.txt

sudo rm -rf /var/www/html/*
ls /var/www/html/ >> /tmp/pavan.txt
sudo git clone https://github.com/ppagilla/nginx-app.git /var/www/html/
ls /var/www/html/ >> /tmp/pavan.txt
sudo systemctl restart nginx
