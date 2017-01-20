---
title: 'Froala Demo'
visible: false
---

This page uses markdown with a couple of so called "Editable sections" which author's can edit using a WYSIWYG editor right on this page. To do so an author needs to be logged in to the front end of the website.

To edit the regions on this page log in to the site and return to this page.

Below are four editable sections. For this demo the editable content is between each 'Marker start' and 'Marker end' line pair.

___
Marker start Editable section 'Child Hero'
[editable name="hero" /]
Marker end Editable section 'Child Hero'
___
Marker start Editable section 'Root Hero'
[editable name="/hero" /]
Marker end Editable section 'Root Hero'
___
Marker start Editable section 'Child NormaDef'
[editable name="normaldef" /]
Marker end Editable section 'Child NormaDef'
___
Marker start Editable section 'Root Solo'
[editable name="/solo" /]
Marker end Editable section 'Root Solo'

___

The "About us" text below is from the page "/about_us". You can edit the content of the "About us" page right here. Try it and then go to the About us page to view your changes.
[editable name="/about-us" /]

The error message here is due to referencing a page which does not exist.
[editable name="gone" /]

Some footer text...

