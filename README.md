# \<fabric-import\>

[![Build Status](https://travis-ci.org/printminion/fabric-import.svg?branch=master)](https://travis-ci.org/printminion/fabric-import)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/printminion/fabric-import)
Element providing solution for including fabricjs library.

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

## Usage

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="fabric-import.html">
    <fabric-import></fabric-import>
    
    <canvas id="canvas" width="300" height="300"></canvas>
    
    <script>
        var seedElement = document.querySelector('fabric-import');
        var canvas = document.querySelector('#canvas');
        var canvasEditorBase = null;
    
        document.querySelector('#dotestbtn').addEventListener('click', function () {
            generateDemo();
        });
    
    
        function generateDemo() {
            console.log('generateDemo');
    
            if (!fabric) {
                alert('failed to include fabricjs');
            }
    
            if (!canvasEditorBase) {
                canvasEditorBase = new fabric.Canvas(canvas);
            }
    
            var width = canvas.width;
            var height = canvas.height;
    
            canvasEditorBase.selection = false;
            canvasEditorBase.clear();
            canvasEditorBase.add(
                    new fabric.Rect({
                        top: getRandomInt(20, height - 20),
                        left: getRandomInt(10, width - 20),
                        width: 40,
                        height: 40,
                        originX: 'center',
                        originY: 'center',
                        fill: '#f55'
                    }),
                    new fabric.Circle({
                        top: getRandomInt(20, height - 20),
                        left: getRandomInt(10, width - 20),
                        radius: 20,
                        originX: 'center',
                        originY: 'center',
                        fill: 'green'
                    }),
                    new fabric.Triangle({
                        top: getRandomInt(20, height - 20),
                        left: getRandomInt(10, width - 20),
                        width: 40,
                        originX: 'center',
                        originY: 'center',
                        height: 40,
                        fill: 'blue'
                    })
            );
    
    
        }
    
        function getRandomInt(min, max) {
            return Math.floor(Math.random() * (max - min + 1)) + min;
        }
    </script>
  </template>
</custom-element-demo>
```
-->
```html
<fabric-import></fabric-import>
```

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.


## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
