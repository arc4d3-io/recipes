# Packer
## install 
```

curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo dd of=/etc/apt/trusted.gpg.d/hashicorp-archive-keyring.gpg
sudo chmod go+r /etc/apt/trusted.gpg.d/hashicorp-archive-keyring.gpg
sudo apt-add-repository -y "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt update && sudo apt install packer
```

## packer + proxmox template

```
git clone https://github.com/arc4d3-io/devops.git
cd devops/packer/proxmox/ubuntu-server-jammy
```

## running machine build

```
packet init
packer build -var-file=../credentials.pkr.hcl ubuntu-server-jammy.pkr.hcl
```

## DEBUG
````
PACKER_LOG=1 packer build -var-file=../credentials.pkr.hcl ubuntu-server-jammy.pkr.hcl
```