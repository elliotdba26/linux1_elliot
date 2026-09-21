# Generate key
sh-keygen -t ed25519 -C "your_name"

# In git bash
ssh-copy-id -i ~/.ssh/id_ed25519.pub kokchun@192.168.1.159

# in ssh. disable password auth
sudo vim /etc/ssh/sshd_config

Disable PasswordAuthentication no
