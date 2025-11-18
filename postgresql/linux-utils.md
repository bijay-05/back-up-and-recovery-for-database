# Few Linux Utilities exercised during the process

```bash
$sudo useradd <username>
$sudo passwd <username>

## change the shell of a user, alternatively `chsh`
$sudo usermod -s /bin/bash <username>

## add a user to sudoers
$sudo usermod -aG sudo <username>
$sudo adduser <username> sudo

## install postgresql client utilities
$sudo apt install postgresql-client

## install ping
$sudo apt install inetutils-ping

## install ip 
$sudo apt install iproute2
```