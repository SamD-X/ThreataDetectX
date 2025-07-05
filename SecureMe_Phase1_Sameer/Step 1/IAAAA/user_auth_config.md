Step 1 : Creating 3 Users : sudo useradd -m user1 , sudo useradd -m user2 , sudo useradd -m user3

Step 2 : Setting Password for Users : sudo passwd user1 , sudo passwd user2 , sudo passwd user3

Step 3 : Creating Test File : touch demo.txt
                              echo "Confidential Info" > demo.txt

Step 4 : Using chmod to manage permissions : chmod 600 demo.txt (Only Owner can Read/Write)

Step 5 : Read Access of file to everyone : chmod 644 demo.txt

Step 6 : sudo usermod -aG sudo user1 (Adding User1 to Sudo)

Step 7 : su - user1
         sudo ls /root

         


 


