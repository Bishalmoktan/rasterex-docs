---
sidebar_position: 3
title: How to add to HTML?
---

Add rxcorefunctions.min.js as a JavaScript reference in the header of the HTML document:

```html
<script type="text/javascript" src="rxcorefunctions.min.js" charset="utf-8"></script>
```

By default, the RxCore object will look for a div with ID 'rxcontainer'. You can specify any div by passing its ID to the RxCore.initialize() method.

### Required CSS

The following CSS declaration must be referenced in the main HTML document:

```css
#rxcontainer {
    position: relative;
    width: 100%;
    height: 100%;
    display: block;
    margin: 0;
    padding: 0;
    border: 0;
    float: left;
}
```

Additional CSS styles for canvas elements:

```css
#rxcanvas { border: 1px solid #000; }
#imageDiag { position: absolute; top: 1px; left: 1px; }
#imageTemp { position: absolute; top: 1px; left: 1px; }
#canvas {
    position: absolute; top: 1px; left: 1px;
    background: -webkit-linear-gradient(#FFFFFF, #b5b5b5); /* Safari 5.1-6.0 */
    background: -o-linear-gradient(#FFFFFF, #b5b5b5);      /* Opera 11.1-12.0 */
    background: -moz-linear-gradient(#FFFFFF, #b5b5b5);    /* Firefox 3.6-15 */
    background: linear-gradient(#FFFFFF, #b5b5b5);         /* Standard syntax */
}
```
