<p align="center">
<img src="app/images/logo.jpg" title="protect eyes app logo" alt="layout of protect eyes app">
</p>



# <p align="center">👁‍🗨 Protect your eyes desktop app (Electron)</p>
<p align="center">Project for learning Electron (building desktop apps using JavaScript, HTML and CSS))</p>

</br>

## Table of Contents

- [What's this project about?](#about)
- [Technologies used](#technologies)
- [What I learned?](#what)
- [Interesting code snippet](#interesting)
- [Installation and quick start](#install)

</br>

## <a name="about"></a>What's this project about?

This is desktop application for measuring the time spent in front of the monitor. Informs you about the time for a break and looking far ahead for 20 seconds. For the good health of your eyes :)

</br>

## <a name="technologies"></a>Technologies used
- Electron
- HTML
- CSS
- JavaScript
- React
- GIT

</br>

## <a name="what"></a>What I learned?
- w



</br>

## <a name="interesting"></a>Interesting code snippet (for me of course 😉)
- Electron setup:

```js
'use strict';

const path = require('path');
const { app, BrowserWindow } = require('electron');

function main() {

  // create new window
  let mainWindow = new BrowserWindow({
    webPreferences: {
      nodeIntegration: true
    },
    width: 520,
    height: 640,
    frame: false,
  })

  // load app/index.html as the window content
  mainWindow.loadFile(path.join('app', 'index.html'));
}

app.on('ready', main);

app.on('window-all-closed', function () {
  app.quit();
});
```

</br>

## <a name="install"></a>Installation and quick start

- use the package manager [npm](https://www.npmjs.com/get-npm) or [yarn](https://classic.yarnpkg.com/en/) to install dependencies:

```bash
npm install // yarn install

or

npm i
```
- run desktop app:

```bash
npm start

or

yarn start
```

</br>
</br>

  *project implemented as part of the 9-month [Web Developer Plus](https://kodilla.com/pl/bootcamp/webdeveloper/?type=wdp&editionId=309) course organized by [Kodilla](https://drive.google.com/file/d/1AZGDMtjhsHbrtXhRSIlRKKc3RCxQk6YY/view?usp=sharing).
