```bash
ssh root@1.2.3.4
apt install sudo
sudo passwd root
apt install curl
curl -sfL https://get.k3s.io | sh -
# Install cert-manager if needed, use the latest release
# kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.12.17/cert-manager.yaml
apt install ufw # 'sudo apt update' might be needed
sudo ufw allow 22
sudo ufw allow 6443 #k8s
sudo ufw allow 500
sudo ufw allow 4500
sudo ufw enable
# apply ufw
reboot
cat /etc/rancher/k3s/k3s.yaml
# update the ip address (don't use domain), convert to base64 and update the werf secret
apt install git
curl -sSL https://werf.io/install.sh | bash -s -- --version 1.2 --channel stable
converge
kubectl exec -n vpn-production -it ipsec-vpn-server-84b65bbc75-87qt6 -- sh
ikev2.sh --addclient username
ikev2.sh --exportclient username
kubectl cp -n vpn-production ipsec-vpn-server-84b65bbc75-87qt6:/etc/ipsec.d/ ./
# copy the config, modify OnDemandRules and import to the OS (the command can produce errors, ignore)
# the array should contain one element 'Connect'
#<key>OnDemandRules</key>
#<array>
#  <dict>
#  <key>Action</key>
#  <string>Connect</string>
#  </dict>
#</array>
```
