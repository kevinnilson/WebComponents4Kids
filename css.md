# CSS

![CSS3 Logo](images/css3logo.png)

**CSS** tells the browser how each type of **HTML** element should be displayed (color, size, font).  **CSS** stands for **C**ascading **S**tyle **S**heets.



## CSS Example

```css
body {
    background-color: #FF0000;
}

h1 {
    color: green;
    text-align: center;
}

p {
    font-family: font-family: "Comic Sans MS", "Comic Sans", cursive;
    font-style: italic;
}
```
The above **CSS** will make your page's background red, the heading will be green and centered, and the paragraph will be cursive and italic.

[try on plunker](http://plnkr.co/edit/0mIhNvQ8fGF0VWvpgnNo?p=preview)







## Ways to Insert CSS
There are 3 ways to add styles
* External style sheet
* Internal style sheet
* Inline style


### External Style Sheet
External style allow you to put your styles in there own files for maintainability.

```html 
<link rel="stylesheet" href="mystyle.css">
```

[try on plunker](http://plnkr.co/edit/fen6KwOWV1ghucIlOomw?p=preview)




### Internal Style Sheet
Internal style sheets allow you to put your styles in the **HTML** file's head.

```html
<head>
  <style>
      h1{
        color:red;
      }
    </style>
</head>
```

[try on plunker](http://plnkr.co/edit/3YGGCJduQGetaxMQ4UmL?p=preview)





### Inline Style
Inline styles allow you to put styling directly in a tag.

```html
<h1 style="color:red;">I love inline styles</h1>```

[try on plunker](http://plnkr.co/edit/PpVdbdftjsRKVDq6K5gN?p=preview)



 

## CSS Selectors
You can limit what is styled with **CSS** selectors.  **CSS** selectors are used to find **HTML** elements based on their: 

* type
* id
* class
* attribute
* ...

```html
<!DOCTYPE html>
<html>

  <head>
    <style>
      /* All h1 tags are red */
      h1{
        color:red;
        text-align: center;
      }
      
      
      /* All tags with the class mycolor are lime */
      .mycolor{
        color:lime;
      }
      
      /* The tag with the id myothercolor are brown */
      #myothercolor{
        color:brown;
      }
    </style>
  </head>

  <body>
    <h1>tag css selector</h1>
    
    <div class="mycolor">using class css selector</div>
    <div id="myothercolor">using id css selector</div>
    
  </body>

</html>

```


[try on plunker](http://plnkr.co/edit/nh2mZt43tMENWDXTeHRC?p=preview)



You can select by type by adding a tag.
```css
h1{
  color:red;
  text-align: center;
}```



You can select by **class** by adding a **.** followed by the class name and adding the **class** to the tag.  Many elements on a page can have the same class.
```css
.mycolor{
    color:lime;
}
```

```html
<div class="mycolor">using class css selector</div>
```


You can select by **id** by adding a **#** followed by the **id** name and adding the *id* to the tag.  Each element with an **id** must have a unique **id**.
```css
#myothercolor{
    color:brown;
}
```
```html
<div id="myothercolor">using id css selector</div>  
```
---
### Learning More
http://www.w3schools.com/css/default.asp