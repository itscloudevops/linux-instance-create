# Launch linux-ec2-instance & Deploy website 👨‍💻


### 1. Name and tags

```
my-linux-instance
```

### 2. Go to AMI

Choose free linux image version


### 3. Instance type

```
t2.micro
```

### 4. Key pair

Create a new keypair👇  or You can use existing keypair

```
my-linux-key.ppk
```

### 5. Network settings

Click edit  ---->   VPC = default or custom

Subnet  = ap-south-1A  or No Preference

Auto-assign public IP  =  Enable

Firewall (security groups)  =  Create a new security group   or You can use existing security group

- ssh   =  anywhere
- http  =  anywhere
- https =  anywhere

### 6. Configure storage

No need to customize anything

### 7. Number of instances

Your choice , example :- 1

##### Launch Instance😊😊😎😎👍✌️


### 8. Connect your instance

Copy Instance Public IPv4 address  and paste it on host name section ( putty )

Click on SSH ( putty )  ---->  Again Click on AUTH  ( putty )   ---->  Now Click on Credentials   ---->  private key file authentication = my-linux-key.ppk

Click on Open  --->  Click on Accept

Login As 👇

```
ec2-user
```
