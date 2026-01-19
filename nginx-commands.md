# test config for syntax errors
sudo nginx -t    

# reload without restarting server
sudo systemctl reload nginx   


# FILES FOR CONFIGURATION (cd)
# main config
/etc/nginx/nginx.conf          

# site configs
/etc/nginx/sites-available/   

# active site configs (usually symlinks) 
/etc/nginx/sites-enabled/     