# toiletKit UI custom elements

### Status
[![NPM Version](https://img.shields.io/npm/v/toiletkit-cusom-elements.svg)](https://www.npmjs.com/package/toiletkit-cusom-elements) [![Greenkeeper](https://travis-ci.org/toiletKit/custom-elements.svg?branch=master)](https://travis-ci.org/toiletKit/custom-elements) [![Greenkeeper badge](https://badges.greenkeeper.io/toiletKit/custom-elements.svg)](https://greenkeeper.io/)  [![Dependency Status](https://img.shields.io/david/toiletKit/custom-elements.svg)](https://david-dm.org/toiletKit/custom-elements) [![License](https://img.shields.io/github/license/mashape/apistatus.svg)]()

[![Build Status](https://saucelabs.com/browser-matrix/dgt41.svg)](https://saucelabs.com/beta/builds/1450dab56fdd45afa7bb9a611c28b6b9)

### UI components using modern technologies

This is a collection of some common front end components. They are developed with the new W3C standard: custom elements. Each component is using plain and optimized javascript for performance. Also the HTML markup (wherever possible) is reduced to offer a great benefit for front end developers).

### Installation

You can install this package by using NPM:
```bash
$ npm i toiletkit/custom-elements
```

### Configuration

The prefix of all the elements is configuarable. To do so duplicate the file `settings.yaml` and name the new file as `settings-custom.yaml`. Open the file in your editor and change the prefix to your taste. (It needs to be one word - check the W3C speifications for valid custom element naming).
Build your custom elements by executing:
```bash
$ grunt
```
The folder named `dist` contains all your elements.

### Usage

For each component that you need to have available in your page you need to add the custom element in the head of the document:
```html
<link href="tk-alert.min.css" rel="stylesheet">
<script src="tk-alert.min.js"></script>
```

### Tests

Once again we are using the great tools from the polymer team here!
You will need `wct` (web component tester) installed globally. To do so just run `npm install web-component-tester -g`.
You might need to run that command as sudo!
After that, in the root folder of this project just run `wct` and see the status of the tests...

The default setup is based on MacOS system and looking for Chrome, Firefox and Safari browsers, you can change this by editing line 5 of https://github.com/toiletKit/custom-elements/blob/master/wct.conf.json#L5

### Browser support

Although all the major browsers are **committed** to support custom elements some of the **all green browsers** do need a polyfill. The polyfills can be found in the dist folder and are created by the Polymer team (Polymer is a Google project).
The repo for the actual polyfill is: https://github.com/webcomponents/webcomponentsjs

### Documentation and demos
Fully documented [here](https://toiletkit.github.io/custom-elements)

### License
Code released under the [MIT License](https://github.com/toiletKit/custom-elements/blob/master/LICENSE).


