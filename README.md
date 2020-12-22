# mysql-backup-script
First create a script file and give this file executable permission.

```

cd /etc/cron.daily/

touch /etc/cron.daily/dbbackup-daily.sh

chmod 755 /etc/cron.daily/dbbackup-daily.sh

vi /etc/cron.daily/dbbackup-daily.sh

```

`Warning: If your password has special charactors in it the use single quotes around it`

Then copy file code lines into file. 

#### Restore database using following command

`gunzip < db_backup_file.gz | mysql -u yourdbuser -p yourdbname`
