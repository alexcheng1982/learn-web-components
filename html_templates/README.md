
HTML Templates
================

Use `<template>` element to create HTML templates. Template needs to be added to the main document tree to display. Use `content` property to acess template's DOM fragment.

Following code shows basic usage of HTML templates.

```javascript
var template = document.querySelector('#user-template');
var userNode = template.content.cloneNode(true);
containerNode.appendChild(userNode);
```