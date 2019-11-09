from ubuntu:16.04
maintainer jaejunkim<catsoar@gmail.com>
run apt-get update
run apt-get install -y nginx
run echo "\ndaemon off;" >> /etc/nginx/nginx.conf
run chown -R www-data:www-data /var/lib/nginx
volume ["data", "/etc/nginx/site-enabled", "/var/log/nginx"]
wordir /etc/nginx
cmd ["nginx"]
expose 80
expose 443
