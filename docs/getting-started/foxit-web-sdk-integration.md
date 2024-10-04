---
sidebar_position: 4
title: Foxit Web SDK Integration
---

For the Foxit version, an additional iframe must be included under the rxcontainer div, using foxpage.html as the source:

```html
<iframe id="foxitframe" src="foxpage.html" width="100%" height="100%" style="position: absolute; top: 0px; left: 0px; z-index: 2; visibility: visible;"></iframe>
```

Foxpage.html references an open-source class that provides the connection with the Foxit web SDK called iframefoxit.js. This uses methods from the Foxit web SDK. Refer to the included Foxit web SDK documentation for details on available methods.