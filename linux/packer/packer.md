# Packer
## install 
```
wget -O- -q https://apt.releases.hashicorp.com/gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/keyring-hashicorp.gpg
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt update && sudo apt install packer
```