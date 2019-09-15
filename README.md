# Project psd2bank

## Installation instructions

#### 1. Download code
`git clone https://github.com/nedialkom/psd2bank`
#### 2. Enter working directory
`cd psd2bank`
#### 3. Obtain .env and .env.db files and place in root directory
#### 4. Stop other web servers as Apache
`sudo service apache2 stop`
#### 5. Start web server
`sudo docker-compose up -V -d --build`
#### 6. Configure apache2
Start Apache with `sudo service apache2 start`.
In `/etc/apache2/sites-available/000-default.conf` add
`Redirect / https://psd2bank.tk/`
at the end of `<VirtualHost *:80>` section
#### 7. Stop web server
`docker-compose down -v`