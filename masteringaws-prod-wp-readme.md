# Deployment Steps
#  Install LAMP
:we have to write a script for Lamp installation 
by using shell script:
 * sudo yum update
 * sudo yum install httpd mariadb105-server php
 * sudo systemctl start httpd mariadb105-server php
 * sudo systemctl enable httpd mariadb105-server php
 * cd /var/www/html
 * After installing lamp to run this shell script we have to grant permission to lamp.sh:
 * sudo chmod +x lamp.sh
 * to run this script : ./lamp.sh

# Install connector:
* sudo yum install php8.4-mysqlnd.x86_64
* cd /var/www/html
* sudo wget https://wordpress.org/latest.tar.gz
* tar -xvzf <file_name>

# Check the application
* http://<pub_ip>/wordpress
![alt text](<Screenshot 2025-07-02 154736.png>)
![alt text](<Screenshot 2025-07-02 155532-1.p ng>)
# Create database
* mysql -u root -p
* create database wordpressdb;
* add information on wordpress
* database name : wordpressdb
* username: root
* password: root
* database host: localhost
* submit
![alt text](<Screenshot 2025-07-02 155709-1-1.png>)

* grant permission to wordpress directory
sudo chmod -R 777 wordpress
* click on submit
* site title: TechBlog
* username: root
* password: root
* write a blog
![alt text](<Screenshot 2025-07-02 192352-1.png>)
