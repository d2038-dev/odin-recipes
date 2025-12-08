# HTML Fundamentals

Basic HTML document structure with DOCTYPE, head, and body elements.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Odin Recipes</title>
  </head>
  <body>
    <!-- Content here -->
  </body>
</html>
```

Unordered list for recipe links.

```html
<ul class="recipes">
  <li><a href="recipes/tequeños.html">Tequeños</a></li>
  <li><a href="recipes/arepas.html">Arepas</a></li>
  <li><a href="recipes/marquesa.html">Marquesa de Chocolate</a></li>
</ul>
```

Image element with source and alt text.

```html
<img
  class="main-image"
  src="./images/odin.jpg"
  alt="Odin holding a spoon and food, with the text 'Odin Recipes' below"
/>
```

# External CSS Method

Linking an external stylesheet in the HTML head.

```html
<link rel="stylesheet" href="style.css" />
```

# Color/Background Properties

Setting background and text colors on the body element.

```css
body {
  background-color: #ffc96f;
  color: #2b2b2b;
}
```

Background color for the container div.

```css
.container {
  background-color: #ffa62f;
}
```

# Typography/Fonts

Importing Google Fonts and setting font-family.

```css
@import url("https://fonts.googleapis.com/css2?family=Cinzel:wght@400..900&display=swap");

body {
  font-family: "Cinzel", "Roboto", "Georgia", serif;
}
```

Setting font-weight for text elements.

```css
.description,
.ingredients,
.steps {
  font-weight: 500;
}
```

# Additional CSS Fundamentals

Universal selector for box-sizing to include padding and borders in element dimensions.

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}
```

Centering content with width, margin, and text-align.

```css
.container {
  width: 80%;
  margin: 0 auto;
  text-align: center;
  padding: 22px;
}
```

Styling links with color inheritance and hover effects.

```css
a {
  color: inherit;
}

a:hover {
  color: #ffe8c8;
}
```

Customizing list appearance by removing default styling.

```css
.recipes {
  padding: 0;
  list-style-type: none;
}
```

Styling an image with width, border, and border-radius.

```css
.main-image {
  width: 50%;
  border: 5px solid #acd793;
  border-radius: 20px;
}
```

Creating a gradient horizontal rule.

```css
hr {
  width: 75ch;
  border: 0;
  height: 1px;
  background-image: linear-gradient(
    to right,
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0.75),
    rgba(0, 0, 0, 0)
  );
}
```
