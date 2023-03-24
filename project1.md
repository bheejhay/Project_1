# Awesome documentation of project 1: LAMP Stack Implementation.


## Step 1: Registering Ssh key generated and Connecting my local system to ec2 instance.
#### In this section the ssh was generated using the ssh-keygen -t ed25519 cmd which is a key-based authentication, you first need to generate public/private key pairs for your client. ssh-keygen.exe is used to generate key files and the algorithms. Then the key genrated was added to the ssh-agent for easy authentication when using it subsiquently. 
![ssh key genrated](./Images/Registering%20my%20ssh%20key%20generated%20into%20ssh%20agent.png "ssh key generated and saved in ssh agent.")

### Part2: Connecting my ec2 instance
#### In this section i connected my ubuntu instance which i lauched on the aws platform to my local machine which enabled me to use it remotely. Any time i stop and restart ec2 instance my ip address changes.
![Connecting ec2 instance](./Images/connecting%20to%20my%20ec2%20instance..png "connecting ec2 instance done successfully")


## Step 2:  Apache installation
#### In this section we successfully installed the Apache2 webserver which is among the most popular web servers in the world. list of packages was updated first in package manager using sudo apt update then followed by the run apache2 package installation using the sudo apt install apache2 cmd.

![Apache installation](Images/Installing%20Apache%20using%20Ubuntu%E2%80%99s%20package%20manager.png  "Apache installation") 

### Part 2: Getting Apache2 installaton status

#### After which we installed the apache2 successfully we had to check the if the web server was successfully installed using the sudo systemctl status apache2 cmd.

![confirmation status of Apache2](./Images/Confirmation%20of%20Apache2%20%20working%20perfectly.png "Apache status")
#### In this section apache was installed successfully.
![Apache2 installed successfully](./Images/Apache2%20being%20installed%20Succefully..png "Apache status: states successful")

## Step 3:  Mysql installation
####  MySQL is a popular relational database management system used within PHP environments its been used to store and manage data for our website. And the cmd been used is the "sudo apt install mysql-server" 
![mysql installation](./Images/installing%20mysql%20server%20cmd.png "mysql installation successfull.")

### part2: confirmation of the installation of mysql.
#### After which we installed the mysql database we had to run another cmd to confirm the installation using the $ "sudo mysql" cmd

![Apache2 Confirmation](./Images/Confirmation%20of%20Apache2%20%20working%20perfectly.png "Apache confirmation")


## Step 4: installation of PHP
#### After installing Apache2 which is to serve my  content and also MySQL has been installed to store and manage my data. PHP is the component of the setup that will process code to display dynamic content to the end user. The cmd "sudo apt install php libapache2-mod-php php-mysql" is been used to install php server.

![installation of PHP ](./Images/Installing%20PHP%20successfully%20done.png "PHP Installation")

### Part 2: confirmation of PHP installed
#### After installing the php server  we had to confirm the the installation of the server in which we used the cmd "php -v" to check.

![confirmation of php](./Images/Virtual%20host%20successfully%20created%20using%20apache.png "Php Confirmation")


## Step 5: Creation of Virtual Host with the Apache2.

#### After which i have installed PHP server and also the Apache server i can launch a website called projectlamps so i made a folder in the directory of the wwww using the cmd " sudo chown -R $USER:$USER /var/www/projectlamps"

![virtual host created](./Images/Virtual%20host%20successfully%20created%20using%20apache.png "creation of virtual host")

### Part 2: PHP Reloaded
#### Now that you have a custom location to host your website’s files and folders, we’ll create a PHP test script to confirm that Apache is able to handle and process requests for PHP files. using the cmd "vim /var/www/projectlamp/index.php" and after which the apache was relaoded.

![PHP Relaoded](./Images/PHP%20sucessfully%20reloaded.png "PHP Relaoded")

### Part 3: Website Loaded on the Browser
#### the website was loaded on the browser to confirm the php and apache installation and the dafault page of the php was removed from the landing page.


![Website Loaded](./Images/webiste%20loaded%20on%20browser.png "Website loaded")


##### This is the complete step in implementing a Lamp stack Project and also lauch it on the Browser.