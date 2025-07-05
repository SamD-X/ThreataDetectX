Step 1 : echo "This is a secure file." > demo2.txt

Step 2 : sha256sum hash1.txt

Step 3 : echo "File content edited." >> demo2.txt

Step 4 : sha256sum demo2.txt > hash2.txt

Step 5 : diff hash1.txt hash2.txt