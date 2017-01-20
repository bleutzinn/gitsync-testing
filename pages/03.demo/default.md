---
title: 'Demo'
cache_enable: false
---

[editable name="hero" /]



Onder deze regel staat een zogenaamde **editable section** (die een div gebruikt voor [Froala](//froala.com):

[plugin:editable](hero?template=modular/editable)

_En hieronder staat een editable section die z'n content haalt uit de modular page 'maintext' zonder template parameter en dus wordt de default template ('modular/editable') gebruikt:_

> [plugin:editable](maintext)

Below this line the content of the page 'Solo' should appear:
[plugin:editable](/solo)

**BEGIN FOOTER**

f o o t e r

**END FOOTER**