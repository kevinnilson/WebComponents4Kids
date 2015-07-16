# Build Your Own Website with Polymer Starter Kit

## Change the Title
app/index.hmtl line 19

```<title>Web Components 4 Kids Project</title>```

[see it on github](https://github.com/kevinnilson/polymer-starter-kit/commit/baf72b4299ce2d5983f0b95f25cf83b2d32fa4e8)

## Change the App Name
app/index.hmtl line 104

```<div class="app-name">Web Components 4 Kids Project</div>```

[see it on github](https://github.com/kevinnilson/polymer-starter-kit/commit/90a4a3ea98c1fe3172a7f6ec3d110d8b0944b98d)

## Add a Card
```html
<paper-material elevation="1">
  <p class="paper-font-body2">This is the card content.</p>
</paper-material>

```
[see it on github](https://github.com/kevinnilson/polymer-starter-kit/commit/87e22866f97d7b5f19e3c8613554774c183d6696)


## Add a Section

app/index.html line 77
```html
<a data-route="devoxx4kids" href="/devoxx4kids">
  <iron-icon icon="devoxx4kids"></iron-icon>
  <span>Devoxx4Kids</span>
</a>
```

app/index.html line 133
```html
<section data-route="devoxx4kids">
  <paper-material elevation="1">
    <h2 class="paper-font-display2">Devoxx4Kids</h2>
    <p>I love Devoxx4Kids!!!</p>
  </paper-material>
</section>
```

app/elements/routing.html line 22
```html
page('/devoxx4kids', function () {
  app.route = 'devoxx4kids';
});
```

[see it on github](https://github.com/kevinnilson/polymer-starter-kit/commit/4aaea5806f9c0f45987309c42388966c9c4fd20b)

### Icons
Look at all the **[Polymer Iron Icons](https://elements.polymer-project.org/elements/iron-icons?view=demo:demo/index.html)** for the menu.


## Change the Theme
https://www.materialpalette.com/