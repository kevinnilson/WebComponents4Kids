# CSS

![CSS3 Logo](images/css3logo.png)

CSS tells the browser how each type of HTML element should be displayed (color, size, font).  CSS stands for Cascading Style Sheets.



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
The above CSS will make your page's background red, the heading will be green and centered, and the paragraph will be cursive and italic.

[try on plunker](http://plnkr.co/edit/0mIhNvQ8fGF0VWvpgnNo?p=preview)







## Ways to Insert CSS
There are 3 ways to add styles
* External style sheet
* Internal style sheet
* Inline style


## External Style Sheet
External style allow you to put your styles in there own files for ease of maintainability.

```html 
<link rel="stylesheet" href="mystyle.css">
```

[try on plunker](http://plnkr.co/edit/fen6KwOWV1ghucIlOomw?p=preview)




## Internal Style Sheet
Internal style sheets allow you to put your styles in the HTML file's head.

```html
<head>
  <link rel="stylesheet" href="mystyle.css">
</head>
```

[try on plunker](http://plnkr.co/edit/3YGGCJduQGetaxMQ4UmL?p=preview)





## Inline Style
Inline style sheets allow you to put styling directly in a tag

```<h1 style="color:red;">I love inline styles</h1>```

[try on plunker](http://plnkr.co/edit/PpVdbdftjsRKVDq6K5gN?p=preview)



 

## CSS Selectors
* element
* id
* class

```html

<!DOCTYPE html>
<html>

  <head>
    <style>
      /* All h1 tags are red */
      h1{
        color:red;
      }
      
      
      /* All span tags are red */
      .mycolor{
        color:lime;
      }
      
      /* All span tags are red */
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

http://plnkr.co/edit/nh2mZt43tMENWDXTeHRC?p=preview


---
### Learning More
http://www.w3schools.com/css/default.asp