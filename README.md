# E-MENU

## Prerequisites

### Polymer CLI

Install [polymer-cli](https://github.com/Polymer/polymer-cli):

    npm install -g polymer-cli

### Setup

    # Using CLI
    mkdir e-menu
    cd e-menu
    polymer init e-menu

    # Or cloning direct from GitHub
    git clone https://github.com/neoformalex/e-menu.git
    cd e-menu
    bower install
    bower install paper-search --allow-root option

## Start the development server

    polymer serve

## Run web-component-tester tests

    polymer test

## Build

Build presets provide an easy way to define common build configurations in your `polymer.json` file. There are 3 build presets we put in `polymer.json` file in E-menu:

**es5-bundled**

- js: {minify: true, compile: true}
- css: {minify: true}
- html: {minify: true}
- bundle: true
- addServiceWorker: true
- addPushManifest: true
- insertPrefetchLinks: true

**es6-unbundled**

- js: {minify: true, compile: false}
- css: {minify: true}
- html: {minify: true}
- bundle: false
- addServiceWorker: true
- addPushManifest: true
- insertPrefetchLinks: true

**es6-bundled**

- js: {minify: true, compile: false}
- css: {minify: true}
- html: {minify: true}
- bundle: true
- addServiceWorker: true
- addPushManifest: true
- insertPrefetchLinks: true

Run the command to build the presets:

    polymer build

## Test the build

Use `polymer serve` to serve a specific build preset of the app. For example:

    polymer serve build/es5-bundled
