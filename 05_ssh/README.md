# Generate key
```bash
sh-keygen -t ed25519 -C "your_name"
```
# In git bash
```bash
ssh-copy-id -i ~/.ssh/id_ed25519.pub your_name@192.168.1.159
```
 
# Disable password auth
```bash
sudo vim /etc/ssh/sshd_config

# Set: PasswordAuthentication no
```
# Restart SSHD
```bash
sudo systemctl restart sshd
``` 

# Remove IP address from ssh command. Edit SSH config file on host 

```bash 
vim ~/.ssh/config/
Host example_name
	HostName ipaddr
	User username
	Port 22
```
# Connect with:
```bash
ssh example_name
```
