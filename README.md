# FRONTEND :

The frontend is the service in Todo to serve the web content over Nginx.

To Update and Install Nginx run below commands.

```
  #apt update

  #apt install nginx 

  #systemctl enable nginx 

  #systemctl start nginx 
```
This service is written in NodeJS, Hence need to install NodeJS in the system.
```
#apt update

#apt install npm -y

$curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -

$sudo apt install nodejs -y
```
Deploy in Nginx Default Location.
```
#cd /var/www/html/

#mkdir todoapp

#cd todoapp/
```
Lets clone the code from github repository
```
#git clone https://github.com/zelar-soft-todoapp/frontend.git

#cd frontend/

#npm install

#npm run build

#cd /etc/nginx/sites-available/

#cd /var/www/html/todoapp/frontend/
```
NOTE: Configure below environment variable 
```
#export AUTH_API_ADDRESS=http://172.31.29.164:8080

#export TODOS_API_ADDRESS=http://172.31.24.171:8080
```
Finally restart the service once to effect the changes by the below cammand.
```
#systemctl restart nginx

#npm start
```
