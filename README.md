# docker

## Instalación de docker en debian 10

apt install apt-transport-https ca-certificates curl gnupg2 software-properties-common

curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -

add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/debian $(lsb_release -cs) stable"

apt update

apt install docker-ce

## Instalaciòn de docker en ubuntu 20.04

sudo apt-get update

sudo apt-get upgrade 

sudo reboot

sudo apt-get install docker.io

sudo systemctl enable --now docker.service

Este comando da privilegios de ejecucion dentro de un usuario a un programa determinado en este caso a docker

sudo usermod -aG docker <user>

En mi caso mi usuarios es "edwin"

sudo usermod -aG docker edwin

Comprobamos que funciona

edwin@VirtualBox:~$ docker --version

Docker version 19.03.8, build afacb8b7f0
