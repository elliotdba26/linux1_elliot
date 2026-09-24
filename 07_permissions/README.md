# add user
```bash
sudo useradd -m username
```
# Add password
```bash
sudo passwd username
#enter password
```
# See which users are added.
```bash
cat /etc/passwd | grep home
```
# Test script
```bash
vim script
#!/usr/bin/env bash
name='your_name'
echo "hello $name"
```
# add privelage
```bash
chmod u+x script
```
# change owner
```bash
sudo chown username script
```
# So anyone can use the script.
```bash
sudo chmod 755 script
```
# Only the owner can edit the script
```bash
chmod 700 script
# test with ls-l
```
# delete test user
```bash
sudo userdel -r username
# test with "cd.." and then "ls" in "/home". "w" to see active users.
```
