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
 app/index.html line 119
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
  <iron-icon icon="thumb-up"></iron-icon>
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
1. 
Select the desired theme from [materialpalette.com](https://www.materialpalette.com/)
1. 
Download the Polymer version
1. 
Update the root of app/styles/app-theme.html at line 25.

```css
--dark-primary-color:       #FBC02D;
--default-primary-color:    #FFEB3B;
--light-primary-color:      #FFF9C4;
--text-primary-color:       #212121;
--accent-color:             #9E9E9E;
--primary-background-color: #FFF9C4;
--primary-text-color:       #212121;
--secondary-text-color:     #727272;
--disabled-text-color:      #BDBDBD;
--divider-color:            #B6B6B6;
```
[see it on github](https://github.com/kevinnilson/polymer-starter-kit/commit/c44dc4a328522ab7841189a5ef4113e5057b5a91)