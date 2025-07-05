Step 1 : gpg --version 

Step 2 : echo "This is a secret message" > demo.txt

Step 3 : gpg --full-generate-key

Step 4 : gpg --list-keys

Step 5 : gpg -e -r "sp" demo.txt

Step 6 : gpg -d demo.txt.gpg
