# Ubuntu

## Première chose à faire

```bash
sudo apt update && sudo apt upgrade
```

Aller dans settings > Dock > Auto-hide

Utilitaire **make** :

```bash
sudo apt install make
```

Utilitaire **curl** :

```bash
sudo apt install curl
```

## Installer les logiciels et dépendances

### Git

```bash
sudo apt install git
```

### Chrome

Installer Google Chrome depuis le site officiel -> [Link](https://www.google.com/intl/fr_fr/chrome/)

### Anki

Installer Anki depuis le site officiel -> [Link](https://apps.ankiweb.net/)

### MySQL

```bash
sudo apt-get install mysql-server mysql-client
```

Après connection :

```bash
sudo mysqladmin -u root -h localhost password votre_mot_de_passe
```

```bash
sudo -u root -p
```

### MySQL WorkBench

```bash
sudo apt install mysql-workbench
```

### Visual studio code

Installer dans *Ubuntu Software* visual studio code en *snap*

### Spotify

Installer dans *Ubuntu Software* Spotify en *snap*

### Node

Pour une plus grande flexibilité **NVM** est la meilleure solution pour contrôler les versions node.

Installer **NVM** depuis le dépôt Github -> [Link](https://github.com/nvm-sh/nvm)

Il installe également automatiquemement **NPM**

Installer également **Yarn** depuis le site offciel -> [Link](https://classic.yarnpkg.com/fr/docs/install#debian-stable)

### Angular

```bash
npm install -g @angular/cli
```

Vérifier la version

```bash
ng --version~
```

## Java

JDK (development kit):

```bash
sudo apt install default-jdk
```

```bash
javac --version
```

JRE (OpenJDK):

```bash
sudo apt install default-jre
```

```bash
java -versions
```

## Docker

Mettre à jour le système

```bash
sudo apt-get update && sudo apt-get install apt-transport-https ca-certificates curl gnupg2 software-properties-common
```

Ajouter le repo docker

```bash
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -
```

Installer  docker

```bash
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"
```

```bash
sudo apt update && sudo apt-get install docker-ce docker-ce-cli containerd.io
```

Pour parler au daemon

```bash
sudo usermod -aG docker your-user
```

Connection à docker hub

```bash
docker login
```

Installer Docker Compose

```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/bin/docker-compose && sudo chmod +x /usr/bin/docker-compose
```

Vérifier la version avec :

```bash
docker-compose --version
```

### Other

Pour changer de disposition clavier :

QWERTY to AZERTY:

```bash
setxkbmap fr
```

AZERTY to QWERTY:

```bash
setxkbmap us
```
