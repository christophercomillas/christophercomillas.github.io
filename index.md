### Basic
To restart from the command-line, run this command:
```markdown
$ sudo reboot
```
We will run two find commands to set the correct permissions on directories and files:
```markdown
$ sudo find /var/www/ -type d -exec chmod 750 {} \;
$ sudo find /var/www/ -type f -exec chmod 640 {} \;
```
### Nginx

If you are using systemd based Linux distro:
```markdown
$ sudo systemctl restart nginx
```
OR
```markdown
$ sudo systemctl reload nginx
```
To view status:
```markdown
# service nginx status
```
OR
```markdown
$ sudo systemctl status nginx
```

