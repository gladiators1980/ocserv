# **CISCO Project** [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://gitlab.com/limner/bank-tornadowebserver)



This is OCSERV + CENTOS PROJECT.

Version : 1.0

Build : Passing

Author : Amir Masoud Noohi

Language : Bash Script




# **PreRequirements**

For This Project You Need below Requirements :
- VPS with Dedicated IP + root Access
- CENTOS 7 Operating System
- [optional] valid ssl certificate

# **Requirement**

For runnig code.py file You Need to install below pakcage for python  :

- radcli 
- epel-release
- net-tools


```shell
$ yum install net-tools epel-release radcli
```

# **install**
## Step0 : Cloning

First of All Clone the Project : 

```shell
$ git clone https://gitlab.com/limner/CISCO-VPN-SERVICE
$  cd CISCO-VPN-SERVICE/
```

## Step1 : Grant Access

Now We should Grant Access to ocserv.sh and make bash runnable

```shell
$ chmod 777 ocserv.sh
$ sed -i -e 's/\r$//' ocserv.sh
$ ./ocserv.sh
```

### Step1.1 : Edit Encrypting Info

For Changing Encrypting info open ocserv.sh with nano or vim 
then edit line 138-139 and 153-154
CN[138] = organization[139] = Your Comapany Name
CN[153] = Server Ip Address or any A record To IP
organization[154] = Your Comapany Name


## Step2 : Answering Questions

When running the script, you will be asked a series of questions for convenience and default settings.

Answer them.

Wait for the script to finish.

## Step3 : Creating User


Now You Can Create Cisco user with following command.

```shell
$ ocpasswd -c / etc / ocserv / ocpasswd Name
```
# **Usage**
For using This Service You Can use Cisco Anyconnect For any platform

I have Gather All of them in <a href="https://dl.softserver.org/cisco" target="_blank">HERE</a>

# **Support**

Reach out to me at one of the following places!

- Telegram at <a href="https://t.me/amirmnoohi" target="_blank">@amirmnoohi</a>
- Gmail at <a href="mailto:highlimner@gmail.com" target="_blank">highlimner@gmail.com</a>

# **License**

[![License](https://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](http://opensource.org/licenses/mit-license.php)**
- Copyright 2018 © <a href="https://gitlab.com/limner/bank-tornadowebserver" target="_blank">Bank Project</a>.
