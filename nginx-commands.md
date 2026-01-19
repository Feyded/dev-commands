# Developer Commands Cheat Sheet

A simple reference for commonly used nginx commands.


```bash
# test config for syntax errors
sudo nginx -t

# reload without restarting server
sudo systemctl reload nginx


# FILES FOR CONFIGURATION (cd)
# main config
/etc/nginx/nginx.conf

# site configs
/etc/nginx/sites-available/default

# active site configs (usually symlinks)
/etc/nginx/sites-enabled/

# copying from local to server
scp -i ~/.ssh/<filename> -r dist/. root@<server_ip>:/var/www/<folder_name>/dist/


```
