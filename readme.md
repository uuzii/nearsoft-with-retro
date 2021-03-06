# Nearsoft Test

This is a sample of Nearsoft Test

### Setup

##### Prerequisites

First, install [Polymer CLI](https://github.com/Polymer/polymer-cli) using
[npm](https://www.npmjs.com) (we assume you have pre-installed [node.js](https://nodejs.org)) avobe v8.

    npm install -g polymer-cli

Second, install [Bower](https://bower.io/) using [npm](https://www.npmjs.com)

    npm install -g bower

### Configure and start the proxy

We need a proxy to avoid cors issue, install the packgages with this command

    cd nearsoft-with-retro/back/proxy
    npm install cors-anywhere

Run this command to serve the app at `http://localhost:8080/` the command also provides a method for
intercept the frontend requests and add headers to avoid the cors block

    node cors.js

### Configure and serve the api

Donwload the api files install the environment settings with this commands:

    cd nearsoft-with-retro/back/api
    npm install --production

The next command serves the app at `http://localhost:1984/` and provides the api rest for the app:

    npm start

### Start the app locally

Donwload the frontend components with this commands:

    cd nearsoft-with-retro/front
    bower install

The next command serves the app at `http://127.0.0.1:8081/list` and provides basic URL
routing for the app:

    polymer serve

### Navigate trough the app

You have the following views in the app:

1. Home view: `http://127.0.0.1:8081/list`
2. Input view: `http://127.0.0.1:8081/editor`
3. Success view: `http://127.0.0.1:8081/success`

