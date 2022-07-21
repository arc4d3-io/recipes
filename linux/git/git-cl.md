# Git Comand Line (Ubuntu)
## install 
```
curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo dd of=/etc/apt/trusted.gpg.d/githubcli-archive-keyring.gpg
sudo chmod go+r /etc/apt/trusted.gpg.d/githubcli-archive-keyring.gpg
sudo apt-add-repository -y "deb [arch=$(dpkg --print-architecture)] https://cli.github.com/packages stable main" 
sudo apt update
sudo apt install gh
```
# authenticate git
```
gh auth login
```