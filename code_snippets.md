# Code Snippets: Odin Recipes Project

This document extracts and documents selective, reusable code snippets from the Odin Recipes project, focusing on HTML structures and CSS properties. All items are new compared to previous notes, as no prior code snippets were documented. The project builds on HTML foundations with CSS basics, emphasizing properties like color, background-color, and typography, while using external CSS and web-safe fonts with fallbacks.

## HTML Snippets

### Basic HTML5 Structure

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>Odin Recipes</title>
  </head>
  <body>
    <!-- Content here -->
  </body>
</html>
```

- **Key Concept**: HTML foundations with DOCTYPE declaration, meta tags for charset and viewport, and external CSS link for separation of concerns.

### Container and Navigation Structure

```html
<div class="container">
  <h1 class="title">Odin Recipes</h1>
  <img
    class="main-image"
    src="./images/odin.jpg"
    alt="Odin holding a spoon and food, with the text 'Odin Recipes' below"
  />
  <ul class="recipes">
    <li><a href="recipes/tequeños.html">Tequeños</a></li>
    <li><a href="recipes/arepas.html">Arepas</a></li>
    <li><a href="recipes/marquesa.html">Marquesa de Chocolate</a></li>
  </ul>
</div>
```

- **Key Concept**: Semantic HTML with div containers, headings, images with alt text, unordered lists for navigation, and anchor links.

### Recipe Page Structure

```html
<div class="container">
  <h1 class="title">Arepas</h1>
  <img
    class="main-image"
    src="../images/arepas.webp"
    alt="a basket with delicious arepas"
  />
  <h2>Description</h2>
  <p class="description">
    Arepas are a staple in Venezuelan and Colombian cuisine...
  </p>
  <hr />
  <h2>Ingredients</h2>
  <ul class="ingredients">
    <li>2 cups precooked corn meal...</li>
  </ul>
  <hr />
  <h2>Steps</h2>
  <ol class="steps">
    <li>Preheat oven to 410° F.</li>
    <!-- More steps -->
  </ol>
  <a href="../index.html">Home</a>
</div>
```

- **Key Concept**: Structured content with headings, paragraphs, lists (unordered for ingredients, ordered for steps), horizontal rules for separation, and navigation links.

## CSS Properties/Examples

### Global Reset and Box-Sizing

```css
@import url("https://fonts.googleapis.com/css2?family=Cinzel:wght@400..900&display=swap");

*,
*::before,
*::after {
  box-sizing: border-box;
}
```

- **Key Concept**: External font import and universal box-sizing for consistent layout behavior.

### Body Styling with Colors and Typography

```css
body {
  margin: 0;
  background-color: #ffc96f;
  color: #2b2b2b;
  font-family: "Cinzel", "Roboto", "Georgia", serif;
}
```

- **Key Concept**: Background-color and color properties for theme; font-family with web-safe fallbacks (Cinzel from Google Fonts, then Roboto, Georgia, serif).

### Container Styling

```css
.container {
  background-color: #ffa62f;
  width: 80%;
  min-height: 100vh;
  margin: 0 auto;
  text-align: center;
  padding: 22px;
}
```

- **Key Concept**: Background-color for contrast; width, min-height, margin for centering and full-height layout; text-align and padding for spacing.

### Typography and Text Alignment

```css
.title {
  margin-top: 0;
}

.description,
.ingredients,
.steps {
  font-weight: 500;
  text-align: justify;
  width: 75ch;
  margin-left: auto;
  margin-right: auto;
}
```

- **Key Concept**: Font-weight for emphasis; text-align justify for readability; width in ch units for optimal line length.

### Links and Hover Effects

```css
a {
  color: inherit;
}

a:hover {
  color: #ffe8c8;
}
```

- **Key Concept**: Color inheritance and hover color changes for interactive elements.

### Image Styling

```css
.main-image {
  margin: 0;
  width: 50%;
  border: 5px solid #acd793;
  border-radius: 20px;
}
```

- **Key Concept**: Width for responsive sizing; border and border-radius for visual appeal.

### List Styling

```css
.recipes {
  font-weight: 500;
  padding: 0;
  list-style-type: none;
}

li {
  margin: 8px 0;
}
```

- **Key Concept**: Removing default list styles and adding custom margins.

### Horizontal Rule Styling

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

- **Key Concept**: Custom gradient border for subtle separators.

## JS Functions

No JavaScript functions were identified in the project files.
