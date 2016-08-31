Add config file and symlink.

    cd /etc/nginx/sites-available

Create directory for log files.

    cd /var/log/nginx
    mkdir hwtmkstff.com

Create directory for data

    cd /var/www
    mkdir hwtmkstff.com

All the data directories and the files contained within should be owned and writable only by root, but world-readable. This means file permissions of 755 for directories and 644 for files.
