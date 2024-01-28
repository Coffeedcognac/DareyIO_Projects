# Webstack Implementation `The LAMP stack` 
#### Aim: To deploy a website with its running tools on a dedicated webserver
####Tools :  AWS, Apache, MySql sever and PHP , openssh
` Note: this task will be deployed using an AWS cloud provisioned EC2 Instance(ubuntu) `
#### We are going to create a key pair aan use it as a 2 way authentication between our local PC and the ec2 instace we cretate on AWS 
`Note if you will be using  openssh on powershell always generate a .pem key pair`
![Generate Keypair](/PRJCT_1/key_pair.JPG)
![Instance created using keypair](/PRJCT_1/EC2.jpg)
![Instance created using keypair](/PRJCT_1/status_running.JPG)
### Setting up your local windows PC to connect(SSH) to your AWS EC2 instance: Click this link to get a guide to install openssh; https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/openssh.html#openssh-install . This tool will be used in powershell to connect to to the EC2 instance . Also see how to connect to your instance here https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/openssh.html
![install openssh via powershell](/PRJCT_1/install_openssh.JPG)
Connect to your instance `ssh -i <private-key-name>.pem ubuntu@<Public-IP-address>` 
![instance connected via openssh on powershell](/PRJCT_1/instance_connected.JPG)
#### update a list of packages in package manager `sudo apt update` then run apache2 package installation `sudo apt install apache2` and check apache is running using `$ sudo systemctl status apache2`
![instance connected via openssh on powershell](/PRJCT_1/instl_apache.JPG)
#### test connection after setting up security rulles for https
#### Next  we install mysql server `sudo apt install mysql-server` then log in using `sudo mysql`. Now we want to set a password for everytime we log in to my mysql using this query `ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';`






