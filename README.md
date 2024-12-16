# EC2-Instance-DevOps-Roadmap-
EC2 Instance project for DevOps Roadmap 
https://roadmap.sh/projects/ec2-instance

## Create t2.micro E2C Ubuntu machine
## Allow traffic on ports 22 and 80
## Create new key pair for SSH

## Connect to the machine
```chmod 400 <key-pair_name>.pem
ssh -i <key-pair_name>.pem ubuntu@<public_ip>
``` 
## Install nginx and configure
```
sudo apt update
sudo apt upgrade -y
sudo apt install nginx -y
sudo cp index.html /usr/share/nginx/html/
sudo systemctl restart nginx
```

