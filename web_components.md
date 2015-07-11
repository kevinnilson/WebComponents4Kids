# Web Components

**Web Components** are a set of new web standards being produced by Google engineers that allow for the creation of reusable widgets or components in the web. 

Web Components consist of 4 main elements which can be used separately or all together:

* Templates
* Shadow DOM
* Custom Elements
* HTML Imports


## Templates

```html
<!-- this is how you define a template -->
<template id="tpl">
<p>Use templates to hold HTML you would like to use again.  I will add some websites I like to this template.</p>

<ul>
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

```<button>Click Me</button>

<script>
var host = document.querySelector('button');
var root = host.createShadowRoot();
root.innerHTML = 'DO NOT <content></content>!!!';
</script>```



## Custom Elements

Custom Elements = Templates + Shadow DOM.

Without custom elements HTML typically looks like div soup:
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

With custom elements your HTML can look much more readable like:
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


```html
<link rel="import" href="my-library-configuration.html">
<my-library-widget type="best"></my-library-widget>```


---
### Learning More
http://webcomponents.org/
https://dzone.com/articles/introduction-web-components






