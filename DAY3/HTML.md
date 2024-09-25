### HTML Basics for Beginners

- **HTML** (Hyper Text Markup Language)

  - HTML is used to create web pages and documents. It allows you to include **links** that users can click to navigate between pages.
  - It’s a **Declarative Language**—you define what content should be displayed, but not how it should look or behave.
  - HTML creates **markup** to structure a webpage, using elements like `<a>` to link to other pages.

  Example of common HTML elements:

  ```html
  <a>
    <!-- Anchor tag for hyperlinks -->
    <href>
      <!-- Attribute for specifying the URL -->
      <p><!-- Paragraph tag --></p></href
    ></a
  >
  ```

### Interview Tip: Draw the Anatomy of an HTML Page

- Being able to **diagram the structure** of an HTML page is essential for interviews.
- You should be able to **draw the structure in your sleep**. Here’s a basic example:

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <meta http-equiv="X-UA-Compatible" content="ie=edge" />
      <title>HTML 5 Boilerplate</title>
      <link rel="stylesheet" href="style.css" />
    </head>
    <body>
      <script src="index.js"></script>
    </body>
  </html>
  ```

  - **`<!DOCTYPE html>`**: Defines the document type (HTML5).
  - **`<html>`**: The root element that contains all the content of the page.
  - **`<head>`**: Holds metadata (information about the page), such as character encoding, links to CSS files, and the title.
  - **`<body>`**: Contains all the visible content displayed on the web page.

### Class vs. ID: Understanding the Difference

- Multiple elements on a page can share the same **class** to apply the same style or behavior.
- **ID** is unique and can only be used once on a page.

  Example:

  ```html
  <div id="uniqueId" class="sharedClass anotherClass">Content goes here</div>
  ```

  - **`<div>`**: The element type, or "tag," used here to create a block section on the page.
  - **`id`**: Unique identifier for one element.
  - **`class`**: A way to group elements for shared styles.

### Attributes and Hierarchy in HTML

- **Attributes** give more information about an element. Common attributes include `id`, `class`, and `charset`.

  - **`id`**: Uniquely identifies one specific element.
  - **`class`**: Groups multiple elements that share styles or behaviors.
  - **`charset`**: Specifies the character encoding for the document, which determines how text is stored.

  Example of HTML with `charset`:

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <!-- Specifies character encoding (e.g., UTF-8) -->
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Year Up United</title>
    </head>
    <body>
      <!-- Body content here -->
    </body>
  </html>
  ```

  - **`charset`**: Ensures text characters are displayed correctly on the page.
  - **`viewport`**: Ensures the page looks good on mobile devices by controlling how it is displayed on smaller screens.

### Example: HTML Page Structure

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is a paragraph.</p>
    <a href="https://www.example.com">Visit Example</a>
    <script src="index.js"></script>
  </body>
</html>
```

This is the basic structure of an HTML document. The **`<head>`** section contains metadata and links to stylesheets or scripts, and the **`<body>`** section holds the content that users will see on the webpage.

---
