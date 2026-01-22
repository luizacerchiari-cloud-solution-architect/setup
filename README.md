
## Setup

1. [Install Java e Git](#java)  
2. [Install Angular](#angular)  
 
## Java e Git


````Java
Write-Host "Instalação Git, GitHub CLI e Java"

winget install --id Git.Git --source winget --accept-package-agreements --accept-source-agreements
winget install --id GitHub.cli --source winget --accept-package-agreements --accept-source-agreements
winget install --id Microsoft.OpenJDK.17 --source winget --accept-package-agreements --accept-source-agreements

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

> **Nota: Nenhum repositorio neste perfil tem fins de abordar noticias, assuntos politicos, jurídicos, eclesiásticos, ou semelhantes, se houver erros, desconsidere**



> **Objetivo do repositório: Estudos, sem fins politicos ou religiosos**> **Objetivo do repositório: Estudos, sem fins politicos ou religiosos**
