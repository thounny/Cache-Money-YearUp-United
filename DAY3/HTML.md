### HTML Basics for Beginners

- **HTML** (Hyper Text Markup Language)

  - HTML is used to create web pages and documents. It includes **links** that let you navigate between pages.
  - HTML is a **Declarative Language**, meaning it tells the browser what content to display, not how to display it.
  - HTML uses **markup** to structure a webpage, with elements like `<a>` to create links.

  Example of common HTML elements:

  ```html
  <a>
    <!-- Anchor tag for links -->
    <href>
      <!-- Attribute to specify the URL of the link -->
      <p><!-- Paragraph tag --></p></href
    ></a
  >
  ```

- **Structure of an HTML Page** (Essential for Interviews)

  - It’s important to know how to structure an HTML page. This basic structure should become second nature.

  Basic HTML page structure:

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

  - **`<html>`**: The root element of the page.
  - **`<head>`**: Contains metadata and links to stylesheets.
  - **`<body>`**: The visible content of the page goes here.

- **Class vs. ID** (How to Organize Elements)

  - **Class**: Used to group elements together, allowing them to share the same styles or behavior.
  - **ID**: A unique identifier for one element on the page (only used once per page).

  Example of a tag with both class and id:

  ```html
  <tag id="unique" class="group1 group2"> Content here </tag>
  ```

  - `tag`: The name of the element (e.g., `<div>`, `<a>`, `<p>`).
  - `id`: A unique name for one specific element.
  - `class`: A way to classify elements for shared styling or functionality.

- **Understanding Attributes in HTML**
  - HTML elements can have multiple attributes, like `id` and `class`, which help organize and style the content.
  - **`id`** is always unique, while **`class`** can be shared by multiple elements.
    Example:
  ```html
  <div class="students">Student 1</div>
  <div class="students">Student 2</div>
  ```

---
