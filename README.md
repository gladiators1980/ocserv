# **Bank Project** [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://gitlab.com/limner/bank-tornadowebserver)

![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Django.svg)
![Build](https://img.shields.io/bitbucket/pipelines/atlassian/adf-builder-javascript/task/SECO-2168.svg)
![PyPI - Status](https://img.shields.io/pypi/status/Django.svg)
![Read the Docs](https://img.shields.io/readthedocs/pip.svg)

This is Bank Management system using Tornado Web server.

Version : 1.0

Build : Passing

Author : Amir Masoud Noohi

Language : Python Both 2.7 - 3.6.5




# **PreRequirements**

For This Project You Need below Requirements :
- pyhon
- mysql

```shell
$ apt install python mysql
```

# **Requirement**

For runnig code.py file You Need to install below pakcage for python  :

- tornado 
- torndb


```shell
$ pip install tornado torndb
```

# **install**
## Step0 : Cloning

First of All Clone the Project : 

```shell
$ git clone https://gitlab.com/limner/bank-tornadowebserver
$ cd bank-tornadowebserver/server
```

## Step1 : Connect to MySQL and create a database

Connect to MySQL as a user that can create databases and users:

```shell
$ mysql -u root
```
    
Create a database named "bank":
    
```shell
mysql> CREATE DATABASE bank;
```
    
Allow the "bank" user to connect with the password "bank":
    
```shell
mysql> GRANT ALL PRIVILEGES ON bank.* TO 'bank'@'localhost' IDENTIFIED BY 'bank';
```

## Step2 : Create the tables in your new database

You can use the provided bankdb.sql file by running this command:

```shell
$ mysql --user=bank --password=bank --database=bank < bankdb.sql
```

You can run the above command again later if you want to delete the
contents of the bank and start over after testing.

Then now you Must Put Database information in code.py from line 13 - 16

## Step3 : Run the bank project


With the default user, password, and database you can just run:

```shell
$ python code.py
```

If you've changed anything, you can alter the default MySQL settings
with arguments on the command line, e.g.:

```shell
$ python blog.py --mysql_user=amir --mysql_password=noohi --mysql_database=bank
```

# **Usage**

Now For Sending Requests You Have 2 Options :
1. Postman
2. Our Client Code

## POSTMAN :
Download and install <a href="https://www.getpostman.com/apps" target="_blank">**Postman**</a>. 

In our Project We Support Both POST & GET Method for Requesting

You Can See Example Below : 

### GET :


![GET GIF](https://softserver.org/gif/bank-project-Server-GET.gif)



### POST :


![POST GIF](https://softserver.org/gif/bank-project-Server-POST.gif)

## OUR CLIENT CODE:

Just Go To Client Folders and Run Below Code : 

```shell 
$ pip3 install requests
$ python3 client-[METHOD].py
```

### GET :


![GET GIF](https://softserver.org/gif/bank-project-Client-GET.gif)



### POST :


This section has not been completed yet


# **Files**

- <a href="https://gitlab.com/limner/bank-tornadowebserver/blob/master/server/bankdb.sql" target="_blank">`/server/bankdb.sql`</a> : This is Database File
- <a href="https://gitlab.com/limner/bank-tornadowebserver/blob/master/server/server.py" target="_blank">`/server/server.py`</a> : This is main python File
- <a href="https://gitlab.com/limner/bank-tornadowebserver/blob/master/server/NETWORK2.pcapng" target="_blank">`/server/NETWORK2.pcapng`</a> : Wireshark Full Sniffed Packets
- <a href="https://gitlab.com/limner/bank-tornadowebserver/blob/master/server/NETWORK2-filtered.pcapng" target="_blank">`/server/NETWORK2-filtered.pcapng`</a> Wireshark Filtered Packets Just HTTP
- <a href="https://gitlab.com/limner/bank-tornadowebserver/blob/master/client/client-get.py" target="_blank">`/client/client-get.py`</a> This is Client Code With GET Method
- <a href="https://gitlab.com/limner/bank-tornadowebserver/blob/master/client/client-post.py" target="_blank">`/client/client-post.py`</a> This is Client Code With POST Method

# **Support**

Reach out to me at one of the following places!

- Telegram at <a href="https://t.me/amirmnoohi" target="_blank">@amirmnoohi</a>
- Gmail at <a href="mailto:highlimner@gmail.com" target="_blank">highlimner@gmail.com</a>

# **License**

[![License](https://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](http://opensource.org/licenses/mit-license.php)**
- Copyright 2018 © <a href="https://gitlab.com/limner/bank-tornadowebserver" target="_blank">Bank Project</a>.
