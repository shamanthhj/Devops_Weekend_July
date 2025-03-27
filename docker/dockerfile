FROM ubuntu:22.04

# Update package list
RUN apt update 

# Install Apache and wget
RUN apt install apache2 wget -y

# Set working directory to Apache web root
WORKDIR /var/www/html

# Download Yahoo's homepage and save it as index.html
RUN wget http://yahoo.com -O index.html

# Start Apache in the foreground
CMD ["apachectl", "-D", "FOREGROUND"]
