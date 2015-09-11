**Welcome to the Setup-Kali wiki!**
## Setup-Kali
### Atualizar source.list
$ sudo leafpad /etc/apt/sources.list
Adicionar nbo Final

deb http://http.kali.org/ /kali main contrib non-free

deb http://http.kali.org/ /wheezy main contrib non-free

deb http://http.kali.org/kali kali-dev main contrib non-free

deb http://http.kali.org/kali kali-dev main/debian-installer

deb-src http://http.kali.org/kali kali-dev main contrib non-free

deb http://http.kali.org/kali kali main contrib non-free

deb http://http.kali.org/kali kali main/debian-installer

deb-src http://http.kali.org/kali kali main contrib non-free

deb http://security.kali.org/kali-security kali/updates main contrib non-free

deb-src http://security.kali.org/kali-security kali/updates main contrib non-free

Posteriormente:

$ sudo apt-get update
$ sudo apt-get upgrade 

### Adicionar Repositórios
apt-get install python-software-properties
### Next install apt-file
apt-get install apt-file
### Update apt-file.
apt-file update
apt-file search add-apt-repository
### Sua saída deve ser semelhante a este::
### Adicionar Repositórios
apt-get install python-software-properties
### Next install apt-file
apt-get install apt-file
### Update apt-file.
apt-file update
apt-file search add-apt-repository
### Sua saída deve ser semelhante a este::
python-software-properties: /usr/bin/add-apt-repository
python-software-properties: /usr/share/man/man1/add-apt-repository.1.gz
### Install Filezilla FTP Client
apt-get install filezilla filezilla-common -
### instalar SublimeText
### Instalando na versão x64
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_amd64.deb && sudo dpkg -i sublime-text_build-3065_amd64.deb
### Instalando na versão x86
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_i386.deb && sudo dpkg -i sublime-text_build-3065_i386.deb
### instalar SublimeText
### Instalando na versão x64
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_amd64.deb && sudo dpkg -i sublime-text_build-3065_amd64.deb
### Instalando na versão x86
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_i386.deb && sudo dpkg -i sublime-text_build-3065_i386.deb
### instalando nodeJs
apt-get install make python g++
mkdir ~/nodejs && cd $_
wget -N http://nodejs.org/dist/node-latest.tar.gz
tar xzvf node-latest.tar.gz && cd `ls -rd node-v*`
### Instalando PHP 5
## Adicione essas fontes de pacotes em seu arquivo sources.list: Digite o arquivo via:
sudo nano /etc/apt/sources.list
## Adicionar estas linhas no final do arquivo 
deb http://packages.dotdeb.org wheezy-php55 all
deb-src http://packages.dotdeb.org wheezy-php55 all
## Save and close (CTRL-X, “y”, ENTER).
sudo apt-get update
## Rode esse comando
wget http://www.dotdeb.org/dotdeb.gpg
sudo apt-key add dotdeb.gpg
sudo apt-get update
## Instale a última versão do PHP 5
sudo apt-get install php5
## Verifique a Versão Instalada
php -v
## Saída na data de Hoje
PHP 5.6.9-0+deb8u1
### Instalação do Composer
$ cd /usr/src_

$ sudo apt-get install curl php5-cli

$ curl -sS https://getcomposer.org/installer | sudo php

$ sudo mv composer.phar /usr/bin/composer

### Verificar a Versão
$ composer --version

Composer version 1.0-dev () 2015-09-07 16:55:30
### Instalação do MySql Workbench
sudo add-apt-repository ppa:olivier-berten/misc && sudo apt-get update 

sudo apt-get install mysql-workbench 
