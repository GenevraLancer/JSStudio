# JSStudio

Установка full-stack JS frameworks на на ОС Linux Mint 18.1 Serena (MATE 64-bit)

### Установка Node.js и менеджера пакетов npm
Посмотрев красивый график выхода релизов, был выбран последний релиз Node.js 8
![alt text](https://github.com/nodejs/Release/blob/master/schedule.png)

1. Установка дополнительных репозиториев nodesource и nodesource(источники), установка ключа для проверки подлинности репозиториев. Источник https://github.com/nodesource/distributions#debmanual
```bash
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
```
Результат исполнения команды:
```bash
## You seem to be using Linux Mint version serena.
## This maps to Ubuntu "xenial"... Adjusting for you...

## Confirming "xenial" is supported...
+ curl -sLf -o /dev/null 'https://deb.nodesource.com/node_8.x/dists/xenial/Release'

## Adding the NodeSource signing key to your keyring...
+ curl -s https://deb.nodesource.com/gpgkey/nodesource.gpg.key | apt-key add -
OK

## Creating apt sources list file for the NodeSource Node.js v8.x repo...
+ echo 'deb https://deb.nodesource.com/node_8.x xenial main' > /etc/apt/sources.list.d/nodesource.list
+ echo 'deb-src https://deb.nodesource.com/node_8.x xenial main' >> /etc/apt/sources.list.d/nodesource.list

## Running `apt-get update` for you...
+ apt-get update
```
2. Установка nodejs и npm
```bash
sudo apt install -y nodejs
nodejs --version
npm --version
 ```
 Установлены версии `nodejs v8.5.0`и `npm 5.3.0`
 
 3. Обновление npm до последней версии. Источник https://docs.npmjs.com/getting-started/installing-node
 ```bash
 sudo npm install npm@latest -g
 npm --version
 ```
 Установлена версия `npm 5.4.2`
