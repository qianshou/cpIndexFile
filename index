#!/usr/bin/env node

const fs = require('fs');
const process = require('process');
const path = require('path');

const fileName = process.argv[2];
const fromIndex = process.argv[3];
const toIndex = process.argv[4];

const fileSuffix = path.extname(fileName);
const filePrefix = fileName.replace(fileSuffix, '');

for(var i=fromIndex; i<=toIndex; i++){
    var fileNameNew = filePrefix + '_' + i + fileSuffix;
    fs.copyFileSync(fileName, fileNameNew);
}