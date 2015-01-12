# rc-tabs
---

react tabs component

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]
[![gemnasium deps][gemnasium-image]][gemnasium-url]
[![node version][node-image]][node-url]
[![npm download][download-image]][download-url]
[![Sauce Test Status](https://saucelabs.com/buildstatus/rc-tabs)](https://saucelabs.com/u/rc-tabs)

[![Sauce Test Status](https://saucelabs.com/browser-matrix/rc-tabs.svg)](https://saucelabs.com/u/rc-tabs)

[npm-image]: http://img.shields.io/npm/v/rc-tabs.svg?style=flat-square
[npm-url]: http://npmjs.org/package/rc-tabs
[travis-image]: https://img.shields.io/travis/react-component/tabs.svg?style=flat-square
[travis-url]: https://travis-ci.org/react-component/tabs
[coveralls-image]: https://img.shields.io/coveralls/react-component/tabs.svg?style=flat-square
[coveralls-url]: https://coveralls.io/r/react-component/tabs?branch=master
[gemnasium-image]: http://img.shields.io/gemnasium/react-component/tabs.svg?style=flat-square
[gemnasium-url]: https://gemnasium.com/react-component/tabs
[node-image]: https://img.shields.io/badge/node.js-%3E=_0.10-green.svg?style=flat-square
[node-url]: http://nodejs.org/download/
[download-image]: https://img.shields.io/npm/dm/rc-tabs.svg?style=flat-square
[download-url]: https://npmjs.org/package/rc-tabs

## Screenshot

<img src='http://gtms03.alicdn.com/tps/i3/TB1TIJ3HXXXXXcYaXXXR6PQLFXX-816-612.png' width='408'>

## install

[![rc-tabs](https://nodei.co/npm/rc-tabs.png)](https://npmjs.org/package/rc-tabs)

## Feature

### Keyboard

* left and up: switch to previous tab
* right and down: switch to next tab

## Usage

```js
var Tabs = require('rc-tabs');
var TabPane = Tabs.TabPane;

var callback = function(eventKey){

}

React.render(
  (
    <Tabs activeKey="2" onChange={callback}>
      <TabPane tab='tab 1' key="1">first</TabPane>
      <TabPane tab='tab 2' key="2">second</TabPane>
      <TabPane tab='tab 3' key="3">third</TabPane>
    </Tabs>
  ),
  document.getElementById('t2'));
```

## Development

```
npm install
npm start
```

## API 

### Tabs

#### props:

<table class="table table-bordered table-striped">
    <thead>
    <tr>
        <th style="width: 100px;">name</th>
        <th style="width: 50px;">type</th>
        <th>default</th>
        <th>description</th>
    </tr>
    </thead>
    <tbody>
      <tr>
          <td>activeKey</td>
          <td>Object</td>
          <th>first active tabPanel's eventKey</th>
          <td>same with active tabPanel's eventKey</td>
      </tr>
      <tr>
          <td>onChange</td>
          <td>Function(eventKey)</td>
          <th></th>
          <td>called when tabPanel is changed</td>
      </tr>
    </tbody>
</table>

### TabPane

#### props:

<table class="table table-bordered table-striped">
    <thead>
      <tr>
          <th style="width: 100px;">name</th>
          <th style="width: 50px;">type</th>
          <th>default</th>
          <th>description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
          <td>key</td>
          <td>Object</td>
          <th></th>
          <td>corresponding to activeKey</td>
      </tr>
      <tr>
          <td>tab</td>
          <td>String</td>
          <th></th>
          <td>current tab's title corresponding to current tabPane</td>
      </tr>
    </tbody>
</table>

## Test Case

http://localhost:8000/tests/runner.html?coverage

## Coverage

http://localhost:8000/node_modules/node-jscover/lib/front-end/jscoverage.html?w=http://localhost:8000/tests/runner.html?coverage

## License

rc-tabs is released under the MIT license.