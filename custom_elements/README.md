Custom Elements
================

Use `<element>` to create custom elements. Use `register` function to register a custom element.

`x-nice-image` is a custom element for displaying image with URL, title, description and author information.

Use `<link rel="import" href="x-nice-image.html">` to import it into current page, then declare elements.

```html
<x-nice-image src="http://farm6.staticflickr.com/5221/5796757101_e6acb81d64.jpg" 
                    title="Waterfalls" description="Waterfalls"
                    author-name="Sean MacEntee" author-url="http://www.flickr.com/photos/smemon/"></x-nice-image>
```