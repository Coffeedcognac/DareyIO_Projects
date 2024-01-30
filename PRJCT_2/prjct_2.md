## Webstack Implementation (LEMP)
#### Linux, EngineX(nginx), Mysqlserver,PHP.
`We will be using Gitbash as the SSH client and AWS provided ubuntu EC2 instance for this task`
##### Provision your server and ssh into it using Gitbash
#### Note make sure to be in the directory where the .pem file is located or be sure to provide the entire path to were the .pem file is saved, see below.
![EC2](prjct_img/lemp_EC2.jpg)
` ssh -i path/to/your/abc.pem ubuntu@your.public.ip.address`
#### I also went to my working directory . Luckily Gitbash sort of functions like our usual linux terminal so we can `pwd`(point your working directory) on it ; this is to make sure that we are on the same path wher our .pem keypair is stored and run
`ssh -i abc.pem ubuntu@your.public.ip.address`
#### This connects you to your instance and now we we will update our default apps and drives with `sudo apt update` and move on to provision our nginx webserver by installing with `sudo apt install nginx` also checj if status is set to active and running with a green colour using this command `sudo systemctl status nginx`
#### We will proceed to activate port 80 on our ubuntu instance to allow http traffic inbound
![port80](prjct_img/nginx_http.JPG)

Run the curl command to your host machine (ubuntu istance )to test for connectivity; curl https://127.0.0.1:80
if the response returns a html formatted text content , it means the connection is valid. We will return to the PC browser and query https://your.public.ip.address:80. it should look like this webpage below
![nginx webpage](prjct_img/nginx_img.JPG)
