# pwa-113
⚡️Projecto de un yarn 
# 🚀 Progressive Web Applications (PWAs) 

PWA: Aplicación Web Progresiva 🙌

## Features

* ⚙️ Offline mode: It works even when you don't have internet connection.
* ❤️ Add to favorite: Follow your favorite artists from the agenda.
* 🎯 Local notifications: Subscribe to your favorite events, and you will be notified.

## Watch the workshop

This project was made as a part of a workshop about Progressive Web Applications. Check it out if you wanna see explanation of the code.

<a href="https://www.youtube.com/watch?v=de1xiqz-BTE"><img src="./workshop_progressive_web_apps_pennapps.png" /></a>

This project is part of a workshop about Progressive Web Applications I've been doing:

NPM Instalar en un NPM (Node Package Manager) en Windows.
En el manejador de versiones de Node, NVM (Node Version Manager).

Un repositorio online para publicar paquetes de software libre para ser utilizados en proyectos Node.js
proyecto basado en Node — que actualmente incluye los proyectos de aplicaciones web que utilizan Node para su proceso de compilación y generación de archivos — utilizarás la utilidad de linea de comandos (cli) para consumir paquetes desde el repositorio online, un listado gigantesco de soluciones de software para distintos problemas.

## Monorepo
Un monorepo (mono repositorio) es un repositorio único que almacena todo su código y activos para cada proyecto.

## Multi Repo
Los repositorios múltiples, por otro lado, se refieren a organizar sus proyectos cada uno en sus propios repositorios separados. Cuantos más proyectos, más repositorios. Un repositorio múltiple también se conoce como polyrepo.

## npm scripts
Una importante sección de este archivo es scripts. Esta sección define un listado de propiedades que permiten ejecutar comandos dentro del contexto de tu proyecto incluyendo: comandos de otros paquetes listados como dependencias, scripts personalizados, scripts bash, etc.
npm es parte esencial de Node.js, el entorno de ejecución de javaScript en el lado del servidor basado en el motor V8 de Google

## Yarn
Los espacios de trabajo de Yarn le permiten organizar la base del código de su proyecto utilizando un repositorio monolítico (monorepo).
En este artículo, Jorge explica por qué son una gran herramienta y cómo crear su primer monorepo usando Yarn con scripts npm básicos y agregar las dependencias necesarias para cada aplicación.
Los proyectos nuevos debería utilizar repositorios git separados,  para mi servidor back-end y mis clientes front-end, de esta manera organizando el código base.

Son aplicaciones WEB con capacidades de las Apps utilizadas por el celular.

## yarn.lock
Este archivo es auto generado por npm install y es una lista descriptiva y exacta de las versiones instaladas durante tu proceso. No esta destinado a ser leído ni manipulado por los desarrolladores, si no, para ser un insumo del proceso de manejo de dependencias.


* [Workshop: Progressive Web Apps at PennApps (University of Pennsylvania)](https://www.ferreiro.me/blog/workshop-progressive-web-apps-at-pennapps)

## Setup your SSL certificate

To run some PWA features we need to have a secure server.
In order to do that, just simply run:

1. $ yarn setup

```bash
openssl req -x509 -out ./certificates/localhost.cert -keyout ./certificates/localhost.key \
  -newkey rsa:2048 -nodes -sha256 \
  -subj '/CN=localhost' -extensions EXT -config <( \
   printf "[dn]\nCN=localhost\n[req]\ndistinguished_name = dn\n[EXT]\nsubjectAltName=DNS:localhost\nkeyUsage=digitalSignature\nextendedKeyUsage=serverAuth")

```
## How to install and develop locally?

1. Clone this repo locally: `$ git clone https://github.com/ferreiro/facebook-hackathon.git`
2. Go to the project folder and run `yarn install`
3. yarn dev => This will create two servers, one of the backend server and the other one a dev server for the react application.

* For more info check: https://timonweb.com/posts/running-expressjs-server-over-https/
* Also check: https://letsencrypt.org/docs/certificates-for-localhost/

