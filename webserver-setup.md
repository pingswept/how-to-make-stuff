Add symlink and config file.

    cd /etc/nginx/sites-enabled
    ln -s /etc/nginx/sites-available/hwtmkstff.com hwtmkstff.com
    cd /etc/nginx/sites-available
    vim hwtmkstff.com

Paste in contents of config file:

    server {
        server_name .hwtmkstff.com; # . before domain means www and naked domain match
    
        access_log /var/log/nginx/hwtmkstff.com/access.log;
        error_log /var/log/nginx/hwtmkstff.com/error.log;
    
        location / {
            root /var/www/hwtmkstff.com;
            index index.html index.htm;
        }
    }

Create directory for log files.

    cd /var/log/nginx
    mkdir hwtmkstff.com

Create directory for data

    cd /var/www
    mkdir hwtmkstff.com

All the data directories and the files contained within should be owned and writable only by root, but world-readable. This means file permissions of 755 for directories and 644 for files.
