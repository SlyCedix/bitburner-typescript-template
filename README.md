## Extension Recomendations
[vscode-bitburner-connector](https://github.com/hexnaught/vscode-bitburner-connector) ([vscode extension marketplace](https://marketplace.visualstudio.com/items?itemName=hexnaught.vscode-bitburner-connector)) to upload your files into the game

[vscode-eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) to use live linting in editor

[auto-snippet](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.auto-snippet) to automate inserting the file template in `.vscode/snippets.code-snippets`

There is a workspace file in `.vscode` which contains the recommended settings for all of these

## Dependancies
[Node.js](https://nodejs.org/en/download/) required for compiling typescript and installing dependencies

[git](https://git-scm.com) to download the bitburner repo to manage typescript docs for ns functions


## Installation
```
git clone https://github.com/SlyCedix/bitburner-typescript-template.git
npm install
npm run defs
```

## How to use this template
Write all your typescript source code in the `/src` directory

Ensure you are using absolute paths to .js files in your imports or else the game will not recognize your import paths.  
Example: use `import {} from '/lib/helpers.js'` instead of `import {} from './lib/helpers'` 

To autocompile as you save, run `npm run watch` in a terminal

To update your Netscript Definitions, run `npm run defs` in a terminal

Press F1 and Select `Bitburner: Enable File Watcher` to enable auto uploading to the game

## Todo
Create a bitburner script which detects updates to files and restarts the running script automatically