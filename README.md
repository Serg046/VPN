```bash
ssh root@1.2.3.4
apt install sudo
apt install curl
curl -sfL https://get.k3s.io | sh -
apt install ufw
sudo ufw allow 6443
cat etc/rancher/k3s/k3s.yaml | base64
update the werf secret
apt install git
curl -sSL https://werf.io/install.sh | bash -s -- --version 1.2 --channel stable
converge
```
