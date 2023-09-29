```bash
ssh root@1.2.3.4
apt install sudo
sudo passwd root
apt install curl
curl -sfL https://get.k3s.io | sh -
apt install ufw
sudo ufw allow 22
sudo ufw allow 6443
sudo ufw allow 500
sudo ufw enable
# apply ufw
reboot
cat /etc/rancher/k3s/k3s.yaml
# update the ip address, convert to base64 and update the werf secret
apt install git
curl -sSL https://werf.io/install.sh | bash -s -- --version 1.2 --channel stable
converge
```
