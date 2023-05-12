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
 

 

  
  
 
     
