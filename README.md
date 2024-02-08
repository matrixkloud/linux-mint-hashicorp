# linux-mint-hashicorp

```
## Download HashiCorp GPG key and save it to the keyring
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg

## Add HashiCorp repository to the apt sources list with Ubuntu 22.04 code name
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com jammy main" | sudo tee /etc/apt/sources.list.d/hashicorp.list

## Update package lists and install Vagrant
sudo apt update && sudo apt install vagrant && apt install terraform
```
