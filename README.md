# FRONTEND :

The frontend is the service in Todo to serve the web content over Nginx.

To Update and Install Nginx run below commands.

```
  # apt update

  # apt install nginx 

  # systemctl enable nginx 

  # systemctl start nginx 
```
This service is written in NodeJS, Hence need to install NodeJS in the system.
```
# apt update

# apt install npm -y

```
Deploy in Nginx Default Location.
```
# cd /var/www/html/

# mkdir todoapp

# cd todoapp/
```

Lets clone the code from github repository

```
# git clone https://github.com/zs-amrutha/frontend.git

# cd frontend/

# npm install

# npm run build

```
Finally restart the service once to effect the changes by the below cammand.

```
# systemctl restart nginx

# npm start
```
# Screenshots 


![todo5](https://user-images.githubusercontent.com/82360490/116790723-756f9380-aad3-11eb-9081-e075b7727a7c.png)


# default :

![todo](https://user-images.githubusercontent.com/82360490/116790727-7e606500-aad3-11eb-91f0-53e990e623ef.png)

# admin/admin :

![todo3](https://user-images.githubusercontent.com/82360490/116790732-83251900-aad3-11eb-8b24-556d893f431d.png)

```
;) ;) ;)
# RELEASE 0.0.1 -DATE - 03-06-2021
# RELEASE 0.0.3 -DATE - 03-06-2021
# RELEASE 0.0.6 -DATE - 03-06-2021
# RELEASE 0.0.7 -DATE - 03-06-2021
# RELEASE v0.0.1 -DATE - 03-06-2021
# RELEASE 0.0.9 -DATE - 03-06-2021
# RELEASE 0.0.10 -DATE - 03-06-2021
# RELEASE 0.0.11 -DATE - 03-06-2021
# RELEASE 0.0.12 -DATE - 09-06-2021
```
