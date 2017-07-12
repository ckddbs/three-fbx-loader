## three-fbx-loader

Kyle-Larson and Takahiro's [THREE.FBXLoader](https://threejs.org/examples/js/loaders/FBXLoader.js) repackaged as a node module

## install

`npm i --save three-fbx-loader`

## usage

```js

var THREE = require('three')
require('three-fbx-loader')(THREE)

var loader = new THREE.FBXLoader()

loader.load('./path/to/model.fbx', function (geometry) {
  var material = new THREE.MeshNormalMaterial()
  var mesh = new THREE.Mesh(geometry, material)
  scene.add(mesh)
})

```