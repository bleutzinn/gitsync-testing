---
title: 'Add Blog Post'
parent: /blog
pagefrontmatter:
    template: item
    published: true
form:
    name: add-page-form
    fields:
        -
            name: title
            label: 'Title of Blog Post'
            placeholder: null
            autocomplete: true
            type: text
            validate:
                required: true
        -
            name: author
            label: 'Author of Blog Post'
            placeholder: null
            type: text
            validate:
                required: true
        -
            name: content
            label: 'Content of Blog Post'
            size: long
            placeholder: null
            type: textarea
            id: simplemde
            validate:
                required: true
        -
            name: taxonomy.tag
            type: checkboxes
            label: 'Tag for Blog Post'
            options:
                tag1: 'Tag 1'
                tag2: 'Tag 2'
                tag3: 'Tag 3'
                tag4: 'Tag 4'
        -
            name: g-recaptcha-response
            label: Captcha
            type: captcha
            recaptcha_site_key: 6LeyugsUAAAAAM4IQVeDbpTssYOTfARPlXiWJLUw
            recaptcha_not_validated: 'Captcha not valid!'
            validate:
                required: true
        -
            name: images
            type: file
            multiple: false
            destination: '@self'
            accept:
                - 'image/*'
    buttons:
        -
            type: submit
            value: 'Submit Blog Post'
            classes: null
    process:
        -
            captcha:
                recatpcha_secret: 6LeyugsUAAAAAHVGk5YvbX6AxYnvlnQ1lo-YwhHW
        -
            addpage: null
        -
            display: thankyou
---

Enter the title, content (formatted in [Markdown](https://simplemde.com/markdown-guide)) and choose the category tag for the new blog post page.