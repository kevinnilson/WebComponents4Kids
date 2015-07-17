# Web Components

**Web Components** are a set of new web standards being produced by **Google** engineers that allow for the creation of reusable widgets or components in the web. 

**Web Components** consist of 4 main elements which can be used separately or all together:

* Templates
* Shadow DOM
* Custom Elements
* HTML Imports


## Templates

```html
<!-- this is how you define a template -->
<template id="tpl">
  <p>
    Use templates to hold HTML you would like to use again.  
    I will add some websites I like to this template.
  </p>

  <ul>
    <li>webcomponents.org</li>
    <li>polymer-project.org</li>
    <li>JavaClimber.com</li>
    <li>AndyNilson.com</li>
    <li>meetup.com/Devoxx4Kids-BayArea</li>
    <li>devoxx4kids.org</li>
  </ul>
</template>

<!-- this is how you can use a template -->
<script>
  var tpl = document.querySelector('#tpl');
  var clone = document.importNode(tpl.content, true);
  document.body.appendChild(clone);
</script>
```


## Shadow DOM

**Shadow DOM** is a tool that lets the web developer create his or her own hidden encapsulated markup and styles in the same way in which
```<video>``` controls are made.

```html 
<button>Click Me</button>

<script>
var host = document.querySelector('button');
var root = host.createShadowRoot();
root.innerHTML = 'DO NOT <content></content>!!!';
</script>```

[try on plunker](http://plnkr.co/edit/nRcMWfo28ZrsSvlbsTbp?p=preview)


## Custom Elements

Custom Elements = Templates + Shadow DOM.

Without custom elements **HTML** typically looks like div soup:
![Div Soup](images/div-soup-resized.jpg)

```
<div>
  <div></div>
  <div>
    <div></div>
    <div></div>
  </div>
  <div>
      <div>
        <div></div>
        <div></div>
        <div></div>
      </div>
  </div>
</div>

```

With custom elements your **HTML** can look much more readable like:
```
<school-class>
  <class-grade></class-grade>
  <class-teacher>
    <teacher-name></teacher-name>
    <teacher-avatar></teacher-avatar>
  </class-teacher>
  <student-list>
      <class-student>
        <student-name></student-name>
        <student-age></student-age>
        <student-avatar></student-avatar>
      </class-student>
  </student-list>
</school-class>
```

## HTML Imports
**HTML Imports** are a way to include external **HTML** documents and web components on a page without making an Ajax request or loading an iframe. Because of this capability, **HTML** Imports may lead to better page load times, new opportunities to reuse code, and easier integrations.

```html
<link rel="import" href="my-library-configuration.html">
<my-library-widget type="best"></my-library-widget>```


---
### Learning More
http://webcomponents.org/
https://dzone.com/articles/introduction-web-components






