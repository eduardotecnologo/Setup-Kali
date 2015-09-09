# Setup-Kali
#Adicionar Repositórios
apt-get install python-software-properties
#Next install apt-file
apt-get install apt-file
#Update apt-file.
apt-file update
apt-file search add-apt-repository
#Sua saída deve ser semelhante a este::

python-software-properties: /usr/bin/add-apt-repository
python-software-properties: /usr/share/man/man1/add-apt-repository.1.gz

#Install Filezilla FTP Client
apt-get install filezilla filezilla-common -y

#instalar SublimeText
#Instalando na versão x64
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_amd64.deb && sudo dpkg -i sublime-text_build-3065_amd64.deb
#Instalando na versão x86
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_i386.deb && sudo dpkg -i sublime-text_build-3065_i386.deb
#instalando nodeJs
apt-get install make python g++
mkdir ~/nodejs && cd $_
wget -N http://nodejs.org/dist/node-latest.tar.gz
tar xzvf node-latest.tar.gz && cd `ls -rd node-v*`
./configure
make install
#instalando Chromium
sudo apt-get install chromium
#Instalar LAMP com apena um comando
sudo apt-get install lamp-server^
#Instalando phpmyadmin
apt-get install phpmyadmin 
#instalando Chorme
Execute os seguinte comando no terminal:
# wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
# apt-get update
# apt-get install google-chrome-stable




