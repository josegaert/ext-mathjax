ext-mathjax
===========

MathJax extension for SVG-Edit 
You can try a working example at http://svgedit.josegaert.com .

SVG-edit is a fast, web-based, JavaScript-driven SVG drawing editor that works in any modern browser. 
See [here](https://code.google.com/p/svg-edit/ for more information).

Using/installing the extension
---------------------------------
First download [SVG-Edit](http://code.google.com/p/svg-edit/downloads/list) and extract to the folder served by your LAMP.
Then, download the `ext-mathjax.js` and the `mathjax-icons.xml` from this repository and place them the `extensions` folder under your SVG-Edit folder.
No you can enable the mathjax extension on two different ways.

You can enable it by giving it as an option of your URL when you point to SVG-Edit in your browser. Like this:

    /localhost/svgedit/svg-editor.html?extensions=ext-mathjax.js
    
The disadvantage of this is that no other extensions will be loaded. You can find out which extensions are loaded by default by searching in the svgedit.compiled.js. file. Search for `extensions` and you will find an array with all the extensions that are loaded by default.

    extensions:["ext-markers.js","ext-connector.js","ext-eyedropper.js","ext-shapes.js","ext-imagelib.js", "ext-grid.js"]
    
Here you can add `"ext-mathjax.js"` in order to load ext-mathjax together with all other extensions. 
