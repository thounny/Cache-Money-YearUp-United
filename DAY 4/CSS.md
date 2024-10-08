# CSS

CSS (Cascading Style Sheets) is a language used to describe the style of an HTML document. CSS defines how HTML elements should be displayed on a web page.

In CSS:

```css
selector {
  property: value;
}

body {
  background-color: black;
}

.class-name {
  property: value;
}

#id {
  property: value;
}
```

---

## CSS Basics

### CSS Syntax

A CSS rule is made up of a **selector** and **declarations** inside curly braces `{}`. Each declaration contains a **property** and a **value**, separated by a colon `:`.

There’s also a hierarchy when formatted with multiple selectors:

- **tag.class.#id** → `tag` → `.class` → `#id` (from least to most specific).

Example:

```css
body {
  color: black;
  padding: 0.5rem 0.25rem 0.5rem 0.25rem;
}
```

### Common CSS Units

- `in`: inches
- `cm`: centimeters
- `px`: pixels
- `em`: relative to the parent element
- `rem`: relative to the root (usually the `body` element)

#### Example

```css
p {
  font-size: 2rem;
  margin: 20px;
}
```

- `rem` = relative to the root, which is the `body` selector.
- Common units include `px` and `rem`, but you might also use `vh` and `vw` for viewport sizing.

---

### Common CSS Properties

- `color`: Sets the text color.
- `background-color`: Sets the background color.
- `font-size`: Sets the size of the text.
- `padding`: Space inside the element, between the content and the border. Like adding padding inside a box.
- `margin`: Space outside the element, pushing elements away from each other.

#### Example: Padding and Margin (Box Model)

The box model consists of four properties: **top, right, bottom, and left**.

```css
div {
  padding: 10px 15px 10px 15px; /* Padding on all sides */
  margin: 20px 10px; /* Top/Bottom 20px, Left/Right 10px */
}
```

---

## Bootstrap Basics

### What is Bootstrap?

Bootstrap makes it easy to scale websites to fit all types of screens (TVs, laptops, phones, etc.). It helps you build responsive websites quickly.

Bootstrap does it easily for us with its responsive grid system and pre-built styles.

### Bootstrap Grid System

The grid system in Bootstrap uses rows and columns to structure content.

---

### Example: Using Classes and IDs

```html
<h1 id="main-header" class="center-text">Year Up United</h1>
<p class="center-text">Join our program today and boost your career!</p>
```

```css
#main-header {
  font-size: 36px;
  color: navy;
}

.center-text {
  text-align: center;
  color: gray;
}
```

---

### Bootstrap Buttons

```html
<button class="btn btn-primary">Join Year Up</button>
<button class="btn btn-success">Success!</button>
```

---
