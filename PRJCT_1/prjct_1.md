# Webstack Implementation `The LAMP stack` 
#### Aim: To deploy a website with its running tools on a dedicated webserver
####Tools :  Apache, MySql sever and PHP , openssh
` Note: this task will be deployed using an AWS cloud provisioned EC2 Instance(ubuntu) `
#### First step( Setting up your local windows PC to connect(SSH) to your AWS EC2 instance) . Click this link to get a guide to install openssh; https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/openssh.html#openssh-install . This tool will be used in powershell to connect to to the EC2 instance .
#### Create a keypair and use it to build your EC2 instance for a 2 way connection.to note when your instance has been connected ; see a sample below , Also see how to connect to your instance here https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/openssh.html
![instance connected via openssh on powershell](PRJCT_1/instance_connected.JPG)
#### update a list of packages in package manager `sudo apt update` then run apache2 package installation `sudo apt install apache2`
#### test connection after setting up security rulles for https
#### Next  we install mysql server `sudo apt install mysql-server` then log in using `sudo mysql`. Now we want to set a password for everytime we log in to my mysql using this query `ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';`






