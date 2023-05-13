# PROJECT-2
## WEB STACK IMPLEMENTATION 
I started by installing the git bash and running this command
 <ssh -i "CHINYEREPBL.pem" ubuntu@ec2-13-51-250-178.eu-north-1.compute.amazonaws.com>
 i proceeded to install Nginx by running the command <sudo apt install ngnix>
  ![Nginx install](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/5bd3af16-c2f6-4666-919b-35dfdfcaa157)

 ![Nginx running](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/2f656a94-245b-49f3-9207-b793504a751c)
### MYSQL INSTALLATION 
 I did this by running the command
 sudo apt install mysql-server
 then i logged into mysql by running
  sudo mysql
   then i exited by running exit
   Then i proceeded by setting up the root user password with
   ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';
 Then i changed my root user password by following the steps 
 sudo mysql_secure_installation
 changed my password and answered yes to the rest of the questions that came up. That completed the successful installation of mysql for LEMP stack.
 ![MYSQL INSTALL FOR LEMP STACK](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/6fbb0c31-c883-4d6f-a861-dc681180e3a5)
 #### INSTALL PHP
 First of all i installed php-fpm which handles php processing and acts as a border between the php interpreter and webserver. I also installed php-mysql which allows php to communicate with mysql. The comand used for the 2 operations was sudo apt install php-fpm php-mysql
 ##### CONFIGURING NGINX TO USE PHP PROCESSOR
 I created a directory structure within /var/www/ called LEMPSTACK sudo mkdir /var/www/projectLEMP, i assigned ownership of the directory with this sudo chown -R $USER:$USER /var/www/projectLEMP
Then i opened a new configuration file in nginx using nano  sudo nano /etc/nginx/sites-available/projectLEMP
It created a blank file which i pasted the bare bones configuration to. I activated the configuration using this sudo ln -s /etc/nginx/sites-available/projectLEMP /etc/nginx/sites-enabled/
This will tell Nginx to use the configuration when next it is reloaded. Then i disabled default Nginx host with this sudo unlink /etc/nginx/sites-enabled/default
I reloaded so changes could apply. 
 ![LEMP STACK IP](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/fbf28c5a-33cb-45b9-99a8-e9fff86783dc)
 ###### Testing PHP with Nginx
Itested php with Nginix by creating a new php file in my document root. I opened the file and inputed some information into it, then i accessed the page using my domain name on my web browser using the public IP address i set up in my nginx configuration file
 
 
 ####### RETRIEVING DATA FROM MYSQL DATABASE WITH PHP 
 I created an example user on mysql, modified the password and was able to log into the database with thw example user account.
 ![MYSQL ACCESS TO EXAMPLE USER](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/3e40da31-8798-43d5-b03d-32f7576b4a28)
 

                             
 



 

  
  
 
     
