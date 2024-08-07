# Deployment of a website named awesomeweb on localhost using Nginx

Linux Distribution Used : Ubuntu

# Steps
## Step 1: Install Nginx
~~~
sudo apt update
~~~
~~~
sudo apt install nginx
~~~

## Step 2: Start Nginx
~~~
sudo systemctl start nginx
~~~

OR
~~~
sudo service nginx start
~~~

check status of nginx running by
~~~
sudo systemctl start nginx
~~~
OR
~~~
sudo service nginx status
~~~

## Step 3 Create HTML Directory
~~~
sudo mkdir /var/www/html/awesomeweb
~~~

Place index.html in the directory
~~~
sudo nano /var/www/html/awesomeweb/index.html
~~~

Edit index.html file as per your requirement.

## Step 4: Configure Nginx
Create a new configuration file for website
~~~
sudo nano /etc/nginx/sites-available/awesomeweb
~~~

Add the following configuration to the file
~~~
server {
    listen 80;
    server_name awesomeweb;

    root /var/www/html/awesomeweb;
    index index.html

    location / {
        try_files $uri $uri/ =404;
    }
}
~~~

## Step 5: Create a symbolic link to enable the site
~~~
 sudo ln -s /etc/nginx/sites-available/awesomeweb /etc/nginx/sites-enabled/
~~~

## Step 6: Test the Nginx configuration for syntax errors
~~~
 sudo nginx -t
~~~

## Step 7: Reload Nginx to apply the changes
  ~~~
  sudo systemctl reload nginx
  ~~~
OR
~~~
sudo service nginx reload
~~~

## Step 8: Update Hosts File
  ~~~
   sudo nano /etc/hosts
  ~~~

   Add the following line:
   ~~~
   127.0.0.1 awesomeweb
   ~~~

## Step 9: Access the Website
Open a browser and navigate to http://awesomeweb


# Contact:
For any questions, contact Ramananda Naik at ramhnaik@gmail.com



