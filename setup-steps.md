### Install RHEL7.2 minimal

### Install zerotier-one VPN and connect
```bash
curl -o /etc/yum.repos.d/fkooman-zerotier-epel-7.repo https://copr.fedorainfracloud.org/coprs/fkooman/zerotier/repo/epel-7/fkooman-zerotier-epel-7.repo
yum -y install zerotier-one
systemctl enable zerotier-one
systemctl start zerotier-one
zerotier-cli join ##NETWORK_ID_HERE##
```

### Assign IP to host in zerotier interface

### Add host to ansible-playbook
