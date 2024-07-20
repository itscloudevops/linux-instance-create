# Launch linux-ec2-instance & Deploy website 👨‍💻


Create Linux-2 instance

Instance Type = t2.micro

Create a new keypair = mykey.ppk

VPC = default or custom

Subnet  = ap-south-1A  or No Preference

Auto-assign public IP  =  Enable

Firewall (security groups)  =  Create a new security group   or You can use existing security group

- ssh   =  anywhere
- http  =  anywhere
- https =  anywhere

Number of instances = 1

Launch Instance


Connect your instance :-

Copy Instance Public IPv4 address  and paste it on host name section ( putty )

Click on SSH ( putty )  ---->  Again Click on AUTH  ( putty )   ---->  Now Click on Credentials   ---->  private key file authentication = my-linux-key.ppk

Click on Open  --->  Click on Accept

Login As = ec2-user

sudo su

yum update

yum install httpd -y

sudo amazon-linux-extras install php8.0 -y

cd /var/www/html

vi index.html   , Press-i

Copy an paste code inside index.html

How to save :-  press esc  --->  :wq

service httpd start

Copy Instance Public-ip & paste it on Browser 🌏⛳🚀✌️


========================== END========================================

- TERMINATE ALL YOUR RESOURCES
