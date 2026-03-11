## HTML – Complete Notes

### 1. Introduction to HTML

**HTML (HyperText Markup Language)** is the standard markup language used to create web pages and structure content on the web.

* Defines the **structure** of a webpage.
* Uses **tags** to describe elements.
* Works with **CSS** (styling) and **JavaScript** (behavior).

### Features

* Platform independent
* Easy to learn
* Supported by all browsers
* Forms the foundation of web development

---

# 2. Basic Structure of an HTML Document

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Page</title>
</head>
<body>

<h1>Hello World</h1>
<p>This is my first webpage.</p>

</body>
</html>
```

### Explanation

| Tag               | Description          |
| ----------------- | -------------------- |
| `<!DOCTYPE html>` | Declares HTML5       |
| `<html>`          | Root element         |
| `<head>`          | Metadata container   |
| `<title>`         | Page title           |
| `<body>`          | Visible page content |

---

# 3. HTML Tags and Elements

### Tag

Keywords enclosed in angle brackets.

Example:

```html
<p>Paragraph</p>
```

### Element

Combination of **opening tag + content + closing tag**

```html
<p>This is paragraph</p>
```

### Empty Elements

No closing tag.

Examples:

```
<br>
<hr>
<img>
<input>
```

---

# 4. HTML Attributes

Attributes provide additional information about elements.

Syntax:

```html
<tag attribute="value">
```

Example:

```html
<a href="https://google.com">Visit</a>
```

### Common Attributes

| Attribute | Description       |
| --------- | ----------------- |
| id        | Unique identifier |
| class     | Group elements    |
| style     | Inline CSS        |
| title     | Tooltip text      |
| src       | Source of media   |
| href      | Link URL          |
| alt       | Alternative text  |

---

# 5. Headings

HTML provides six levels of headings.

```html
<h1>Main Heading</h1>
<h2>Sub Heading</h2>
<h3>Section Heading</h3>
<h4>Subsection</h4>
<h5>Small Heading</h5>
<h6>Smallest Heading</h6>
```

---

# 6. Paragraph and Text Formatting

### Paragraph

```html
<p>This is a paragraph.</p>
```

### Formatting Tags

| Tag        | Meaning        |
| ---------- | -------------- |
| `<b>`      | Bold           |
| `<strong>` | Important text |
| `<i>`      | Italic         |
| `<em>`     | Emphasized     |
| `<u>`      | Underline      |
| `<mark>`   | Highlight      |
| `<small>`  | Smaller text   |
| `<del>`    | Deleted text   |
| `<ins>`    | Inserted text  |
| `<sub>`    | Subscript      |
| `<sup>`    | Superscript    |

Example:

```html
<p>This is <strong>important</strong> text.</p>
```

---

# 7. HTML Links

Used to navigate between pages.

```html
<a href="https://example.com">Visit Website</a>
```

### Open Link in New Tab

```html
<a href="https://example.com" target="_blank">Open</a>
```

### Link to Email

```html
<a href="mailto:example@email.com">Send Email</a>
```

---

# 8. HTML Images

```html
<img src="image.jpg" alt="Description" width="300">
```

### Attributes

| Attribute | Description    |
| --------- | -------------- |
| src       | Image path     |
| alt       | Alternate text |
| width     | Image width    |
| height    | Image height   |

---

# 9. Lists

### Ordered List

```html
<ol>
<li>HTML</li>
<li>CSS</li>
<li>JavaScript</li>
</ol>
```

### Unordered List

```html
<ul>
<li>Apple</li>
<li>Mango</li>
<li>Orange</li>
</ul>
```

### Description List

```html
<dl>
<dt>HTML</dt>
<dd>Markup Language</dd>
</dl>
```

---

# 10. Tables

```html
<table border="1">
<tr>
<th>Name</th>
<th>Age</th>
</tr>

<tr>
<td>John</td>
<td>25</td>
</tr>
</table>
```

### Table Tags

| Tag   | Description     |
| ----- | --------------- |
| table | Table container |
| tr    | Table row       |
| th    | Table header    |
| td    | Table data      |

---

# 11. Forms

Forms collect user input.

```html
<form>
<label>Name:</label>
<input type="text">

<label>Email:</label>
<input type="email">

<input type="submit">
</form>
```

### Input Types

| Type     | Description   |
| -------- | ------------- |
| text     | Text field    |
| password | Password      |
| email    | Email input   |
| number   | Number input  |
| date     | Date picker   |
| checkbox | Checkbox      |
| radio    | Radio button  |
| file     | File upload   |
| submit   | Submit button |

---

# 12. Semantic HTML

Semantic tags describe meaning of content.

| Tag     | Meaning             |
| ------- | ------------------- |
| header  | Page header         |
| nav     | Navigation          |
| section | Section             |
| article | Independent content |
| aside   | Sidebar             |
| footer  | Footer              |

Example:

```html
<header>
<h1>My Website</h1>
</header>

<nav>
<a href="#">Home</a>
<a href="#">About</a>
</nav>
```

---

# 13. HTML Multimedia

### Audio

```html
<audio controls>
<source src="audio.mp3" type="audio/mpeg">
</audio>
```

### Video

```html
<video width="400" controls>
<source src="video.mp4" type="video/mp4">
</video>
```

---

# 14. HTML Iframe

Embeds another webpage.

```html
<iframe src="https://example.com"></iframe>
```

---

# 15. HTML Entities

Used for reserved characters.

| Entity   | Symbol |
| -------- | ------ |
| `&lt;`   | <      |
| `&gt;`   | >      |
| `&amp;`  | &      |
| `&nbsp;` | Space  |
| `&copy;` | ©      |

---

# 16. HTML Meta Tags

Used for metadata.

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Website description">
```

---

# 17. HTML Global Attributes

Common attributes used in most elements.

| Attribute | Description  |
| --------- | ------------ |
| id        | Unique ID    |
| class     | CSS class    |
| style     | Inline CSS   |
| title     | Tooltip      |
| hidden    | Hide element |

---

# 18. HTML Block vs Inline Elements

### Block Elements

Take full width.

Examples:

```
div
p
h1-h6
section
article
```

### Inline Elements

Take only needed width.

Examples:

```
span
a
img
strong
em
```

---

# 19. HTML Div and Span

### Div (Block)

```html
<div>
<p>Content</p>
</div>
```

### Span (Inline)

```html
<span style="color:red">Red Text</span>
```

---

# 20. HTML Best Practices

* Use **semantic tags**
* Keep code **clean and indented**
* Use **alt attribute for images**
* Avoid **inline CSS**
* Use **external CSS and JS**

---

# 21. HTML5 New Features

* Semantic elements
* Audio and video support
* Canvas graphics
* Local storage
* New input types

---

# 22. Example Complete HTML Page

```html
<!DOCTYPE html>
<html>
<head>
<title>My Website</title>
</head>

<body>

<header>
<h1>Welcome to My Website</h1>
</header>

<nav>
<a href="#">Home</a>
<a href="#">About</a>
<a href="#">Contact</a>
</nav>

<section>
<h2>About</h2>
<p>This is a simple website.</p>
</section>

<footer>
<p>Copyright 2026</p>
</footer>

</body>
</html>
```


# Advanced HTML Notes (Professional Level)

## 1. HTML5 Overview

**HTML5** is the latest major version of HTML that introduced semantic structure, multimedia support, improved forms, APIs, and better browser interoperability.

### Key Improvements

* Semantic elements
* Native multimedia (`audio`, `video`)
* Advanced form controls
* Web APIs
* Offline storage
* Improved accessibility

---

# 2. Semantic HTML (Advanced)

Semantic elements provide **meaningful structure** to a webpage, improving **SEO, accessibility, and maintainability**.

| Element        | Purpose                 |
| -------------- | ----------------------- |
| `<header>`     | Introductory content    |
| `<nav>`        | Navigation links        |
| `<main>`       | Main content            |
| `<section>`    | Thematic grouping       |
| `<article>`    | Independent content     |
| `<aside>`      | Sidebar or related info |
| `<footer>`     | Footer content          |
| `<figure>`     | Media with caption      |
| `<figcaption>` | Caption for media       |

### Example

```html
<header>
  <h1>Tech Blog</h1>
</header>

<nav>
  <a href="#">Home</a>
  <a href="#">Articles</a>
</nav>

<main>
  <article>
    <h2>Web Development</h2>
    <p>HTML5 semantic structure example.</p>
  </article>
</main>

<footer>
  <p>Copyright 2026</p>
</footer>
```

---

# 3. HTML Document Metadata

Metadata provides **information about the webpage** for browsers, search engines, and social media.

### Important Meta Tags

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Learning HTML">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="Author Name">
```

### SEO Meta Tags

```html
<meta name="robots" content="index, follow">
```

---

# 4. HTML Accessibility (a11y)

Accessibility ensures web pages are usable by **people with disabilities**.

### Techniques

* Use semantic elements
* Add `alt` text for images
* Use `label` for form inputs
* Maintain proper heading hierarchy
* Provide keyboard navigation

### Example

```html
<label for="email">Email</label>
<input id="email" type="email">
```

### ARIA Attributes

ARIA improves accessibility for assistive technologies.

| Attribute     | Purpose                  |
| ------------- | ------------------------ |
| `aria-label`  | Accessible label         |
| `aria-hidden` | Hide from screen readers |
| `role`        | Defines element role     |

Example:

```html
<button aria-label="Close Menu">X</button>
```

---

# 5. Advanced Forms

### Example Form

```html
<form action="/submit" method="POST">

<label>Name</label>
<input type="text" required>

<label>Email</label>
<input type="email" required>

<label>Age</label>
<input type="number" min="1" max="100">

<input type="submit">

</form>
```

### Advanced Input Types

| Input Type | Purpose          |
| ---------- | ---------------- |
| `email`    | Email validation |
| `url`      | URL validation   |
| `tel`      | Telephone        |
| `date`     | Date picker      |
| `time`     | Time picker      |
| `range`    | Slider           |
| `color`    | Color picker     |

Example:

```html
<input type="color">
<input type="range" min="0" max="100">
```

---

# 6. Form Validation

HTML5 includes **built-in validation**.

### Attributes

| Attribute   | Function           |
| ----------- | ------------------ |
| `required`  | Mandatory field    |
| `min`       | Minimum value      |
| `max`       | Maximum value      |
| `pattern`   | Regex validation   |
| `maxlength` | Maximum characters |

Example:

```html
<input type="text" pattern="[A-Za-z]{3,}">
```

---

# 7. Data Attributes

Custom attributes used for storing data in HTML elements.

Syntax:

```html
data-*
```

Example:

```html
<div data-user-id="101"></div>
```

Access using JavaScript:

```javascript
element.dataset.userId
```

---

# 8. HTML Multimedia Advanced

### Video Example

```html
<video controls width="500">
  <source src="video.mp4" type="video/mp4">
</video>
```

### Audio Example

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
</audio>
```

### Important Attributes

| Attribute | Function     |
| --------- | ------------ |
| controls  | Show player  |
| autoplay  | Auto play    |
| muted     | Mute sound   |
| loop      | Repeat media |

---

# 9. HTML Graphics

## Canvas

Used for **dynamic graphics via JavaScript**.

```html
<canvas id="myCanvas" width="200" height="100"></canvas>
```

JavaScript Example

```javascript
let canvas = document.getElementById("myCanvas");
let ctx = canvas.getContext("2d");

ctx.fillStyle = "blue";
ctx.fillRect(10,10,150,75);
```

---

## SVG

SVG is **vector graphics in XML format**.

Example:

```html
<svg width="200" height="200">
  <circle cx="100" cy="100" r="50" fill="red"/>
</svg>
```

---

# 10. HTML Storage

## Local Storage

Stores data permanently in the browser.

```javascript
localStorage.setItem("username","John");
```

Retrieve:

```javascript
localStorage.getItem("username");
```

---

## Session Storage

Stores data only during session.

```javascript
sessionStorage.setItem("user","Admin");
```

---

# 11. HTML Lazy Loading

Improves performance by loading images **only when needed**.

```html
<img src="image.jpg" loading="lazy">
```

---

# 12. HTML Picture Element (Responsive Images)

```html
<picture>
  <source media="(min-width:800px)" srcset="large.jpg">
  <source media="(min-width:400px)" srcset="medium.jpg">
  <img src="small.jpg">
</picture>
```

---

# 13. HTML Web APIs

Common APIs used with HTML:

| API               | Purpose            |
| ----------------- | ------------------ |
| Geolocation API   | User location      |
| Drag and Drop API | Drag elements      |
| Web Storage API   | Store data         |
| Web Workers       | Background scripts |

---

# 14. Drag and Drop API

```html
<div draggable="true">Drag me</div>
```

JavaScript handles drop events.

---

# 15. HTML Performance Optimization

Best practices:

* Minimize DOM size
* Use lazy loading
* Optimize images
* Use semantic markup
* Use CDN for assets

---

# 16. HTML SEO Best Practices

* Proper heading hierarchy
* Semantic tags
* Descriptive titles
* Meta description
* Alt attributes for images

Example:

```html
<title>Learn Web Development</title>
<meta name="description" content="Complete web development course">
```

---

# 17. HTML Security Practices

Important security considerations:

### Avoid Inline Scripts

Use external JS files.

### Use HTTPS

Secure data transfer.

### Escape User Input

Prevent **XSS attacks**.

---

# 18. HTML Best Practices (Professional)

* Maintain clean indentation
* Use semantic HTML
* Avoid unnecessary divs
* Keep accessibility standards
* Use external CSS and JS
* Validate HTML with W3C validator

---

# 19. HTML Boilerplate (Professional)

```html
<!DOCTYPE html>
<html lang="en">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Website</title>

<link rel="stylesheet" href="style.css">
</head>

<body>

<header>
<h1>Website Title</h1>
</header>

<main>
<section>
<h2>Main Content</h2>
<p>Content goes here</p>
</section>
</main>

<footer>
<p>Copyright 2026</p>
</footer>

<script src="script.js"></script>

</body>
</html>
```

---

# 20. HTML Interview-Level Topics

Advanced developers should understand:

* Semantic HTML
* Accessibility (ARIA)
* SEO optimization
* Form validation
* Canvas vs SVG
* LocalStorage vs SessionStorage
* Responsive images
* HTML performance optimization

---
