# Project Omega Client - Light PHP MVC

[![Node.js CI](https://github.com/nenuadrian/project-omega-client/actions/workflows/node.js.yml/badge.svg)](https://github.com/nenuadrian/project-omega-client/actions/workflows/node.js.yml)

[![Electron CI](https://github.com/nenuadrian/project-omega-client/actions/workflows/electron.yml/badge.svg)](https://github.com/nenuadrian/project-omega-client/actions/workflows/electron.yml)

# Add key to github 
```
ssh-keygen -t rsa
cat .ssh/id_rsa.pub

git config --global user.email adrian.nenu@gmail.com
git config --global user.name Adrian
```

## Add webhook for auto-deploy

Webhook to `https://domain.com/deploy/deploy` in GitHub hooks e.g. https://github.com/nenuadrian/cardinal/settings/hooks

## Setup

```
rm -rf domain.com
ln -s project-omega/server/public_html domain.com
```

```
curl -sS https://getcomposer.org/installer | php

php composer.phar install

/usr/local/php80/bin/php composer.phar install
```

Then there is a `/setup` screen to install the DB and creating configuration files automagically.

## Setup Locally

Install MAMP https://www.mamp.info/


# Client

Choices between Angular in `angular-client` directory, Desktop Electron-based and HTML in PHP, using `server/src/views/`.

# Install

```
git clone git@github.com:nenuadrian/project-omega.git

git submodule update --init --recursive

git pull --recurse-submodules
```
