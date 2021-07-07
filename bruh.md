# Readme

## 1. Introduction

This is a port of [R-IN-V0.3](http://dblp.uni-trier.de/db/journals/rct-lrec2005/rct-lrec2005.pdf) to javascript.  
It is currently under development.  Please send suggestions for improvement to [javagit](http://github.com/vitorbaptist/javagit).

The port was made using [javagit](http://github.com/vitorbaptist/javagit).  
The port works only on node.js and doesn't use the new browser [canvas2image](http://github.com/zachleat/canvas2image) 
to render the figures.

## 2. Compilation

1. Install grunt from node.js package manager.

```sh
npm install -g grunt-cli
```

2. Install [bower](http://github.com/bower/bower).

```sh
bower install jquery canvas2image
```

3. Install grunt package from node.js package manager.

```sh
npm install -g grunt
```

4. Install bower package from node.js package manager.

```sh
npm install -g bower
```

5. Create the package's directory.

```sh
mkdir rctlib
cd rctlib
```

6. Start the grunt server.

```sh
grunt serve
```

## 3. Usage

- [HTML demo](http://vitorbaptist.github.io/rct)
- [Example of use](http://github.com/vitorbaptist/rct-examples/tree/master/canvas/example.html)


```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Canvas2Image</title>
    <style>
      html, body {
        margin: 0px;
        padding: 0px;
      }
      canvas {
        display: block;
      }
      img {
        width: 200px;
        height: 300px;
      }
    </style>
  </head>
  <body>
    <img src="http://vitorbaptist.github.io/canvas2image/assets/img/demo.jpg" alt="Sample image"/>
    <canvas id="canvas" width="200" height="300"
            style="border: 1px solid black"></canvas>
  </body>
</html>
```
