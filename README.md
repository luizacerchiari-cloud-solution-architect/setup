
## Java, Git, Angular

# Table of contents  
1. [Install Java](#java)  
2. [Install Angular](#angular)  
 
## Java

````Java
#!/bin/bash

echo "Instalando Git, GitHub CLI e Java"

sudo apt-get update -y
sudo apt-get install -y git openjdk-17-jdk curl

curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo dd of=/usr/share/keyrings/githubcli-archive-keyring.gpg
sudo chmod go+r /usr/share/keyrings/githubcli-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null
sudo apt-get update -y
sudo apt-get install -y gh

git --version
gh --version
java -version
````


## Angular
```bash


Write-Host "Instalação Node e Angular - uso pessoal"

if (Get-Command node) {
    node -v
} else {
    winget install OpenJS.NodeJS.LTS --source winget --accept-package-agreements --accept-source-agreements
}

npm install -g npm
npm install -g @angular/cli
node -v
npm -v
ng version

```
