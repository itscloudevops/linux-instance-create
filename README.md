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

### 9. Allow Some Permission In order to Host Website🛠️🏗️

Update your linux instance

```
sudo su
yum update
```

Now Install webserver

```
yum install httpd -y
```


Now Install Framework

```
sudo amazon-linux-extras install php8.0 -y
```


Create and deploy index.html file📄📜

```
cd /var/www/html
```

vi index.html

Press-i

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LwD</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #edf1f5;
        }
        header {
            background-color: #164578;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #7d5a6a;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #575757;
        }
        main {
            padding: 20px;
        }
        footer {
            background-color: #7d5a6a;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to Learn-with-Dev</h1>
    </header>
    <nav>
        
        <a href="#"> ENROLL HERE </a>
        
    </nav>
    <main>
        <h2>About Us</h2>
        <p>We are Providing Multi-Cloud & Devops Online Trainning.</p>
<p>Thank You !!!</p>
    </main>


    <footer>
        <p>&copy; 2024 LWD-community</p>
    </footer>
</body>
</html>

```

How to save :-  press esc  --->  :wq


### 10. Start your Website

```
service httpd start
```

### 11. Access Website Now


Copy Instance Public-ip & paste it on Browser 🌏⛳🚀✌️


========================== END========================================

- TERMINATE ALL YOUR RESOURCES
