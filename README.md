# fonzo-Text-Editor


### Description

This is a web-based text editor that lets you create and save notes or code snippets, even when you're offline. It's equipped with advanced features like an integrated service worker and Cache API to ensure it works seamlessly without an active internet connection. This means you can access your content and visited pages even when you're not connected to the internet.


### Table of Contents

* [Installation](#installation)
* [How to Use](#usage)
* [References](#references)
* [License](#license)

### Installation

To set up this text editor, follow these steps:

1. Install Node.js and necessary npm packages.
2. Run `npm init` to set up your project and generate a `package.json` file with project details.
3. Install the following npm packages using these commands:
   - `npm install express` (express.js)
   - `npm install --save-dev webpack` (Webpack)
   - `npm install webpack-dev-server --save-dev` (webpack-dev-server)
   - `npm install --save-dev webpack-pwa-manifest` (WebpackPwaManifest)
   - `npm install babel` (Babel)
   - `npm install --save-dev css-loader` (CSS-loader)
   - `npm install concurrently --save` (Concurrently)
   - `npm install idb` (IndexedDB)

4. Bundled modules are listed in `package.json`. Install them by running `npm run install` in the CLI or integrated terminal.

### How to Use

1. Run `npm run start` from the root directory to start the backend and serve the client.
2. Launch the text editor application from your terminal. This will bundle your JavaScript files using webpack.
3. When using next-gen JavaScript, the text editor functions without errors in your browser.
4. When you open the text editor, IndexedDB immediately creates a database storage. Any content you enter and click off the DOM window is saved in IndexedDB.
5. Reopening the text editor retrieves your saved content from IndexedDB.
6. Click the "Install" button to download the web application icon to your desktop.
7. Loading the web application registers a service worker using workbox. Static assets are pre-cached upon loading, including subsequent pages and assets.
8. Deploying to Heroku requires proper build scripts for a webpack application.
