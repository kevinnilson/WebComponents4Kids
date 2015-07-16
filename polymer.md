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
TODO ADD PLUNKER


## Advanced Web Component
Define the **Web Component**:
```html
<link rel="import"
      href="http://www.polymer-project.org/1.0/samples/components/polymer/polymer.html">

<dom-module id="my-styled-namecard">
  <style>
    /* This would be crazy in non webcomponents. */
    span {
      font-weight: bold;
    }
  </style>
  <template>
    <div>
      Hi! My name is <span>{{myName}}</span>
    </div>
  </template>

  <script>
    Polymer({
      is: 'my-styled-namecard',
      properties: {
        myName: {
          type: String
        }
      }
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
    <link rel="import" href="my-styled-namecard.html">
  </head>
  <body>
  
    <my-styled-namecard my-name="Kevin"></my-styled-namecard>

  </body>
</html>
```


[try on plunker](http://plnkr.co/edit/T6p6QXoun8mAxdIBnWBa?p=preview)

##Google Web Components
https://elements.polymer-project.org/browse?package=google-web-components

A collection of web components for Google APIs & services. Built with Polymer.

The below example shows how easy it is to add a gogole map to your site using Google Web Components.

```html
<!DOCTYPE html>
<html>
<head>
  <!-- Polyfill Web Components for older browsers -->
  <script src="webcomponents-lite.js"></script>

  <!-- Import element -->
  <link rel="import" href="google-map.html">

  <style>
    google-map {
      height: 600px;
    }
  </style>
</head>
<body>

  <google-map latitude="37.790" longitude="-122.390"></google-map>

</body>
</html>
```

[try on plunker](http://plnkr.co/edit/xGNgPEFDFCN4qsBiEeVt?p=preview)


---
### Learning More
https://www.polymer-project.org/1.0/docs/start/what-is-polymer.html


