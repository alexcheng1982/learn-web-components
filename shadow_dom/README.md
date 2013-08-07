Shadow DOM
================

## Basic Usage

Use `webkitCreateShadowRoot` to create shadow host. 

Use `<content>` to specify insertion points.

This example shows how shadow DOM encapsulate styles.

## Advanced Usage

`x-person-badge` is a custom element which displays a badge for a person.

In the main document tree, only basic information is added.

```html
<x-person-badge>
    <span class="name">Fu Cheng</span>
    <span class="email">alexcheng1982@gmail.com</span>
    <span class="twitter-handle">alexcheng1982</span>
</x-person-badge>
```

`x-person-badge` custom element add extra DOM nodes and styles. The actual rendered DOM is a composition of shadow host's children and shadow tree's children.

Use code like `<content select=".name">` to specify insertion points based on CSS selectors.

Polymer provides `createShadowRoot` function to create shadow root without vendor specific prefix.

`applyAuthorStyles` and `resetStyleInheritance` control how CSS styles are applied when crossing shadow DOM boundary.