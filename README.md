# fabric-import

[![Build Status](https://travis-ci.org/printminion/fabric-import.svg?branch=master)](https://travis-ci.org/printminion/fabric-import)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/printminion/fabric-import)
Element providing solution for including fabricjs library.

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


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/fabric-import/`, where `fabric-import` is the name of the directory containing it.


## Testing Your Element

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/fabric-import/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.


## Yeoman support

If you'd like to use Yeoman to scaffold your element that's possible. The official [`generator-polymer`](https://github.com/yeoman/generator-polymer) generator has a [`seed`](https://github.com/yeoman/generator-polymer#seed) subgenerator.
