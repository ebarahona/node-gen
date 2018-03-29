# node-gen
npm package to create directories and files with basic node templates using touch and mkdir commands.

## Overview
I work with NodeJS for server side applications and manually create modules and JS files although simple and small I got tired of repeating the same small task so I wrote this to automatically generate common files.  This also helps to keep things consistent.

## Install
Download or clone repo
$ cd node-gen
$ npm install -g

## Usage
From any directory where you would like to generate module folders or files
$ node-gen touch <file-name> or <file-name.js>
$ node-gen mkdir module-name

## Notes
Will convert camecase names to dash (hyphen) separated names

## Example output
```javascript
/* jshint node: true, devel: true */
'use strict';


const helloWorld = () => {
  console.log('Hello World');  
};

const API = {
    helloWorld
};

module.export = API;
```

## TODO:
Add more commands
Much more!
