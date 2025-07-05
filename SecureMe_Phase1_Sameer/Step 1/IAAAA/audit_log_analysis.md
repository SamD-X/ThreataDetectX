Step 1 : Viewing recent Authentication Logs : sudo cat /var/log/auth.log | tail -n 50

Step 2 : Viewing Failed SSH Logins : grep "Failed password" /var/log/auth.log

Step 3 : Viewing successful SSH Logins : grep "Accepted password" /var/log/auth.log

Step 4 : Viewing sudo Usage : grep "sudo" /var/log/auth.log

Step 5 : Viewing New User Sessions : grep "session opened" /var/log/auth.log

Step 6 : Viewing Unauthorized Access Attempts : grep "authentication failure" /var/log/auth.log

Step 7 : Viewing by filter logs bu Username: grep "sp" /var/log/auth.log


