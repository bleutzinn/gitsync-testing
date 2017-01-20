---
title: Home
shortcode-core:
    active: false
---

# Editable plugin demo

The Editable plugin enables authors or writers to edit content without having to work in the Admin back end. All edits can be made "in context", that is right on the page as it is shown on the website. 

Out of the box, Editable supports two editors: ContentTools and Froala. These editors allow the admin to configure multiple editable regions on a single page using shortcodes.

In this demo all texts in blue are editable. This is normally not the case and it is up to you, the admin, to decide how you would communicate which regions are editable to your client being the author or writer of content.

To add an editable region two things need to be done:
1. create a new page which will contain the editable content
2. add a shortcode to the page markdown where you want the editable region to appear and set the name attribute to the page you created in step 1.

Suppose you created a page named "Part 1" as a child page of the current page. To use that page as the container of a new editable region use this shortcode:

`[editable name="part-1" /]`

The name or id of the editable region is set by the 'name' parameter of the shortcode and is the filepath of the editable content page, in this case 'part-1'.

