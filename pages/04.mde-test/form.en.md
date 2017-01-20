---
editable:
    editable_self: true
title: 'Add New Page'
template: form
parent: /
pagefrontmatter:
    title: 'My New Page'
    template: page
    visible: true
    course:
        title: 'CMPT363 E100'
        assignment: 'Reading Quiz #1'
    instructor:
        name: 'John Doe'
form:
    name: add-page-form
    fields:
        -
            name: title
            label: 'Page Title'
            placeholder: 'Enter your page title here'
            autocomplete: true
            type: text
            validate:
                required: false
        -
            name: content
            id: simplemde
            label: 'Page Content'
            size: long
            placeholder: 'Write your assignment here'
            type: textarea
            validate:
                required: true
    buttons:
        -
            type: submit
            value: Submit
            classes: null
    process:
        -
            addpage: null
---

<h2>
    Add another page to your website
</h2>
<p>
    The only **thing....**
</p>