Added Support for ExtJS 5.0.x and for Ext.data.BufferedStore.

#Ext.ux.grid.Printer 

##Overview

Ext.ux.grid.Printer is a small library that provides a way of printing Ext Grid Component.

##Installation

Place the folder ux/grid in your project.

##Usage

In your application file, please add the printer to the require array of your component

    ...
    require: [
        'Ext.ux.grid.Printer'
    ],
    ...


Ext.ux.grid.Printer.print just take a single argument - a normal grid instance. Use it like this:

    var myGrid = new Ext.grid.GridPanel({
      //your usual grid config here
    });
    
    var myGridPrinter = Ext.create('Ext.ux.grid.Printer');
    myGridPrinter.print(myGrid);

##Example

Open example.html to see how to use it.

##Custom Options

You can customize some options:

* printAutomatically = false; - to disable the automatic printing (the print window will not open, user will only see the print version of the grid).
* stylesheetPath = '/some/other/path/gridPrint.css'; - to change the path of the css file.
* ...

You need to set the custom config before calling Ext.ux.grid.Printer.print function.

##Demo for extjs4 gridprinter 

http://loianegroner.com/extjs/examples/extjs4-ux-gridprinter/

##Authors

Plugin originally developed by Ed Spencer (Ext JS 3.x)
* http://edspencer.net/2009/07/printing-grids-with-ext-js.html

Plugin ported to Ext JS 4 by Loiane Groner
* http://loianegroner.com (English)
* http://loiane.com (Portuguese)

MIT License (MIT)

Copyright (c) 2015 connors and other contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
