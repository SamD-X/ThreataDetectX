Step 1 : sudo visudo

In this, chek for this line and if missing then add it : Defaults logfile="/var/log/sudo.log"

Step 2 : sudo ls /root
         cat /var/log/sudo.log (we can see an entry)

Step 3 : Confirming rsyslog is running : sudo systemctl status rsyslog


