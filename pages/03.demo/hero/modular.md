---
title: Hero
content:
    items: '@self.modular'
    order:
        by: date
        dir: desc
body_classes: modular
visible: true
form:
    name: comments
    fields:
        -
            name: name
            label: PLUGIN_COMMENTS.NAME_LABEL
            placeholder: PLUGIN_COMMENTS.NAME_PLACEHOLDER
            autocomplete: true
            type: text
            validate:
                required: true
        -
            name: email
            label: PLUGIN_COMMENTS.EMAIL_LABEL
            placeholder: PLUGIN_COMMENTS.EMAIL_PLACEHOLDER
            type: email
            validate:
                required: true
        -
            name: text
            label: PLUGIN_COMMENTS.MESSAGE_LABEL
            placeholder: PLUGIN_COMMENTS.MESSAGE_PLACEHOLDER
            type: textarea
            validate:
                required: true
        -
            name: date
            type: hidden
            process:
                fillWithCurrentDateTime: true
        -
            name: title
            type: hidden
            evaluateDefault: grav.page.header.title
        -
            name: lang
            type: hidden
            evaluateDefault: grav.language.getLanguage
        -
            name: path
            type: hidden
            evaluateDefault: grav.uri.path
    buttons:
        -
            type: submit
            value: PLUGIN_COMMENTS.SUBMIT_COMMENT_BUTTON_TEXT
    process:
        -
            email:
                subject: PLUGIN_COMMENTS.EMAIL_NEW_COMMENT_SUBJECT
                body: '{% include ''forms/data.html.twig'' %}'
        -
            addComment: null
        -
            message: PLUGIN_COMMENTS.THANK_YOU_MESSAGE
        -
            reset: true
---

final
[comment]: # ( Editable content separator )
<p>Child Hero<br /><strong>draft mooi man.</strong> Eens kijken wat er gebeurt nu de processin<u>g of Twig is enabled</u> on this page. Nou niks eigenlijk. Editable werkt gewoon lekker door.</p>