---
title: New
editable:
    editable_self: true
---

## Header

This table is just a way to make some verical room in order to be able to read the remark about the strange Header markup.
| Column 1 | Column 2 | Column 3 |
| -------- | -------- | -------- |
| Text     | Text     | Text     |

This is weird. The markdown "\#\# Header" gets parsed into this HTML : 

```
<h2 id="header">Header</h2>
```

The content which is served by Grav is "clean" so SimpleMDE adds the id? Why?

With any other header text, for example "\#\# Heade" there is no problem at all:

## Heade
Bla bla