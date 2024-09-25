# HTML Basics:

- **HTML (Hypertext Markup Language)**: The core language for creating web pages, interpreted by browsers to structure content visually.
- **HTML Tag Syntax**: Tags are keywords wrapped in angle brackets (`<tag></tag>`), some of which are self-closing (e.g., `<br>`, `<img>`).
  ```html
  <p>This is a paragraph.</p>
  <br />
  <!-- This is a self-closing tag for a line break -->
  <img src="image.jpg" alt="Description of the image" />
  ```
- **HTML Attributes**: Used to provide additional information to tags (e.g., `src` for images, `href` for links, `alt` for accessibility).
  ```html
  <a href="https://yearup.org" target="_blank">Visit Year Up United!</a>
  <img src="image.jpg" alt="A descriptive text for the image" />
  ```
- **Basic Page Structure**:
  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>Page Title</title>
    </head>
    <body>
      <h1>Welcome to My Website</h1>
      <p>This is an example of a basic HTML page.</p>
    </body>
  </html>
  ```

### Common HTML Tags:

- **Headings**: `<h1>` to `<h6>` define different levels of section headings.
  ```html
  <h1>Main Heading</h1>
  <h2>Subheading</h2>
  <h3>Smaller Subheading</h3>
  ```
- **Paragraphs**: `<p>` represents a block of text.
  ```html
  <p>This is a paragraph of text that goes inside a</p>
  <p>tag.</p>
  ```
- **Lists**: `<ul>` for unordered (bulleted), `<ol>` for ordered (numbered), with items wrapped in `<li>`.

  ```html
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>

  <ol>
    <li>First step</li>
    <li>Second step</li>
    <li>Third step</li>
  </ol>
  ```

- **Links**: `<a>` defines a hyperlink.
  ```html
  <a href="https://google.com">Visit Google</a>
  ```
- **Images**: `<img>` embeds images in a webpage.
  ```html
  <img src="cat.jpg" alt="A cute cat" width="300" height="200" />
  ```

### Block vs Inline Elements:

- **Block Elements**: Always start on a new line and take full width (e.g., `<div>`, `<p>`, `<h1>`).
  ```html
  <div>
    <h1>This is a heading inside a div</h1>
    <p>This is a paragraph inside a div</p>
  </div>
  ```
- **Inline Elements**: Take up only as much width as necessary (e.g., `<span>`, `<a>`).
  ```html
  <p>This is a <span style="color:red">red</span> word in a sentence.</p>
  ```

### CSS Basics:

- **CSS (Cascading Style Sheets)**: Used to style HTML elements (e.g., colors, fonts, layouts).
  ```html
  <style>
    p {
      color: blue;
      font-size: 16px;
    }
  </style>
  ```
- **Selectors**: Apply styles to HTML elements:
  - Type selectors:
    ```css
    h1 {
      color: darkgreen;
    }
    ```
  - Class selectors:
    ```css
    .myClass {
      background-color: yellow;
    }
    ```
    ```html
    <p class="myClass">This paragraph has a yellow background.</p>
    ```
  - ID selectors:
    ```css
    #myId {
      font-size: 20px;
    }
    ```
    ```html
    <div id="myId">This text is styled by the ID selector.</div>
    ```

### Box Model:

- **Box Model**: Every element is a rectangular box consisting of content, padding, border, and margin.
  ```css
  div {
    width: 300px;
    padding: 10px;
    border: 5px solid red;
    margin: 20px;
  }
  ```

### Bootstrap Basics:

- **Grid System**: Bootstrap uses a 12-column grid system.
  ```html
  <div class="container">
    <div class="row">
      <div class="col-md-4">Column 1</div>
      <div class="col-md-4">Column 2</div>
      <div class="col-md-4">Column 3</div>
    </div>
  </div>
  ```
- **Responsive Images**: Use `img-fluid` class to make images responsive.
  ```html
  <img src="image.jpg" class="img-fluid" alt="Responsive image" />
  ```
- **Utility Classes**: Use predefined classes for spacing, text alignment, and more.
  ```html
  <div class="mt-3 text-center">
    This div has a top margin and centered text.
  </div>
  ```

### Additional Code Examples:

#### External CSS with a Linked File:

```html
<head>
  <link rel="stylesheet" href="styles.css" />
</head>
```

#### Using a CSS Class for Multiple Elements:

```css
.text-center {
  text-align: center;
}
```

```html
<p class="text-center">This paragraph is centered.</p>
<h2 class="text-center">This heading is also centered.</h2>
```

#### Flexbox Example:

```css
.container {
  display: flex;
  justify-content: space-around;
}
.box {
  width: 100px;
  height: 100px;
  background-color: lightblue;
}
```

```html
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

---
