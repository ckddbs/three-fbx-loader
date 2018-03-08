## three-fbx-loader

Kyle-Larson and Takahiro's [THREE.FBXLoader](https://threejs.org/examples/js/loaders/FBXLoader.js) repackaged as a node module

## install

`npm i --save three-fbx-loader`

## usage

```js

var THREE = require('three');
var FBXLoader = require('three-fbx-loader');

var loader = new FBXLoader();

var scene = new THREE.Scene();

loader.load('./path/to/model.fbx', function (object3d) {
  scene.add(object3d);
});

```