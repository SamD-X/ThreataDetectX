Step 1 : Generating SSH Key Pairs : ssh-keygen -t rsa -b 4096

Step 2 : keeping Privte Key Secret and Copying Public Key to the Server :

mkdir -p ~/.ssh
cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys

Step 3 : Configuring sshd_config : sudo nano /etc/ssh/sshd_config

Step 4 : Restarting SSH Service : sudo systemctl restart ssh

Step 5 : Now, testing SSH Key Based Login : ssh eth0 (or other ip)
Here, it will not ask for Password instead it will checks if the connecting client has the correct private key.

