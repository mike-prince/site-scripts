# site
Basic shell script to quickly setup and control sites with Nginx.

The script makes certain assumptions about where files are located, but this can be easily changed.  The default path variables are:

```
sites_dir=/srv/www/
sites_available_dir=/etc/nginx/sites-available
sites_enabled_dir=/etc/nginx/sites-enabled
service_dir=/etc/systemd/system
git_dir=/srv/git
```

## Usage

Output can also be obtained with ```site help```.

```
  Usage: site [command] <args>

  Commands:
    site | site help    Output this help information
    site backup         Backup the given site(s)
    site backup-all     Backup all sites
    site delete         Backup and delete the given site(s)
    site disable        Disable the given site(s)
    site enable         Enable the given site(s)
    site list           Output site list and status
    site new            Setup the directories and Nginx configuration for the given site(s)
    site permissions    Set owner www-data, directories 755 and files 644
    site repo           Setup repo for Git deployment
```
