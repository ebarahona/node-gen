# node-gen
npm package to create directories and files with basic node templates using UNIX like commands touch and mkdir.

## Overview
I work with NodeJS for server side applications and manually create modules and JS files, although simple and small I got tired of repeating the same small task so I wrote this to automatically generate common files.  This also helps to keep things consistent. Why "node-gen" because "ed-cli" was already taken.

## Install
Download or clone repo then:

$ cd node-gen

$ npm install -g

## Usage
From any directory where you would like to generate module folders or files
## Quick Overview

```sh
npx create-react-app my-app
cd my-app
npm start
```

Create module - will create directory and index.js inside directory

```sh
node-gen mkdir <module-name>
```

$ node-gen touch <file-name> or <file-name.js>

$ node-gen mkdir <module-name>

## Notes
Will convert camelcase names to dash (hyphen) separated names

## Example output file
```javascript
/* jshint node: true, devel: true */
'use strict';

/**
 * Required Dependencies 
 * go here
 */

const helloWorld = () => {
  console.log('Hello World');  
};

const API = {
    helloWorld
};

module.export = API;
```

## TODO:
Clean up

Add template options ie; --html, --js etc..

Add more commands

Add tests

Much more!
