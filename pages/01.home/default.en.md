---
title: Home
shortcode-core:
    active: false
shortcode-core.merged: null
---

## Editable plugin demo !!!

The **Editable plugin** allows writers or authors to edit content without accessing the website administration back end. All edits can be done right on the page in the front end. [comment]: # (just a comment)

This should save immediately. It does. And these changes should appear on GitHub as well. They do, I noticed on GitHub where I typed this sentence.

Out of the box, Editable supports two editors ContentTools and Froala. Both support "in context" editing, that is content can be edited right on the page. Which editor is used can be configured in the plugin configuration.

Website administrators can add editable regions to a page by inserting one or more shortcodes in the page markdown. An Editable shortcode typically looks like:

`[editable name="part-1" /]`

An explanation of the shortcode syntax plus examples is included in the [Editable shortcode Guide](shortcode-guide).
ContentTools allows per session edits only. That means that all edits must be saved before leaving the page that is being edited. When using Froala edits are automatically stored as draft content and working on draft texts can span multiple sessions and so even several days. The drawback of using draft texts is that caching must be disabled. **At the moment, there is yet no front end UI for approving draft texts.**

This is just some text to test the Git Sync plugin ...

