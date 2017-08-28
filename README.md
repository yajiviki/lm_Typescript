# Use TypeScript for Adobe Products
## Prerequisites
Install [Node.js](https://nodejs.org/en/download/) and [TypeScript](https://www.typescriptlang.org/#download-links).

## Your first script for eg. Adobe Illustrator
```
mkdir test
cd test
npm init -y
npm i pravdomil/types-for-adobe
printf '{"compilerOptions":{"module":"none","noLib":true,"types":["types-for-adobe/illustrator"]},"exclude":["node_modules"]}' > tsconfig.json
printf 'app.activeDocument' > index.ts
tsc -p .
# open index.ts your favourite TypeScript editor and start scripting
# run index.js in Adobe Illustrator
# change tsconfig.json types value to Adobe product you're targeting
```

## Note
Declaration files is generated by https://github.com/pravdomil/extendscript-xml-to-typescript converter.

Definitions was created in summer 2017 by [Pravdomil.com](https://pravdomil.com).
You can [buy a beer for him](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=BCL2X3AFQBAP2&item_name=types-for-adobe%20Beer).
