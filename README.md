# Password-Auditing-with-John-the-Ripper

Install John the Ripper:
sudo apt install john  # Install password cracker

.Create a password file for testing:
echo "user1:5f4dcc3b5aa765d61d8327deb882cf99" > test_passwords.txt  # MD5 hash of "password"

Crack the password:
john --format=raw-md5 test_passwords.txt  # Specify hash format

View results:
john --show test_passwords.txt  # Display cracked passwords
