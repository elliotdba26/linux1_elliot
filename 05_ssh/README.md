# Generate key
bash```
sh-keygen -t ed25519 -C "your_name"
```
# In git bash
bash``` ssh-copy-id -i ~/.ssh/id_ed25519.pub your_name@192.168.1.159```
 
# in ssh. disable password auth
```bash sudo vim /etc/ssh/sshd_config

Disable PasswordAuthentication no
```
# Restart SSHD
```bash sudo systemctl restart sshd``` 

# Remove IP address from ssh command
