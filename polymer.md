# Polymer

The **Polymer** library is designed to make it easier and faster for developers to create great, reusable components for the modern web.


**Polymer** builds on top of the **upcoming** web components technologies. Not all browsers support these standards yet, so the [web components **polyfill** library](http://webcomponents.org/polyfills/) fills the gaps, implementing the **API**s in **JavaScript**. As these technologies are implemented in browsers, the polyfills will shrink and you'll gain the benefits of native implementations.



## Simple Web Component
Define the **Web Component**:
```html
<link rel="import"
      href="http://www.polymer-project.org/1.0/samples/components/polymer/polymer.html">

<dom-module id="dom-element">

  <template>
    <p>I'm a DOM element. This is my local DOM!</p>
  </template>

  <script>
    Polymer({
      is: "dom-element"
    });
  </script>

</dom-module>

```

Use the **Web Component**:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <script src="http://www.polymer-project.org/1.0/samples/components/webcomponentsjs/webcomponents-lite.min.js"></script>
    <link rel="import" href="dom-element.html">
  </head>
  <body>
    <dom-element></dom-element>
  </body>
</html>
```


[try on plunker](http://plnkr.co/edit/T6p6QXoun8mAxdIBnWBa?p=preview)

##Google Web Components
https://elements.polymer-project.org/browse?package=google-web-components


---
### Learning More
https://www.polymer-project.org/1.0/docs/start/what-is-polymer.html


