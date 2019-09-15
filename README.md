# Project psd2bank

## Installation instructions

#### Download code
`git clone https://github.com/nedialkom/psd2bank`
#### Enter working directory
`cd psd2bank`
#### Obtain .env and .env.db files and place in root directory
#### Stop other web servers as Apache
`sudo service apache2 stop`
#### Start web server
`sudo docker-compose up -V -d --build`
#### Stop web server
`docker-compose down -v`