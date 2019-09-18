FROM nginx:1.14

# Copy httpd.conf with changes to the root directory
COPY default.conf /etc/nginx/conf.d/

# Copy the following directory
COPY sample/ /usr/share/nginx/html/sites