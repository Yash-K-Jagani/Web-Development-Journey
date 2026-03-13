---

# CSS Complete Notes

## 1. Introduction to CSS

**CSS (Cascading Style Sheets)** is used to style and layout web pages.

It controls:

* Colors
* Fonts
* Spacing
* Layout
* Animations
* Responsiveness

CSS works with **HTML** to improve the visual appearance of web pages.

Example:

```html
<p style="color:red;">Hello World</p>
```

---

# 2. Types of CSS

## 1. Inline CSS

Applied directly inside an HTML tag.

```html
<p style="color: blue;">Hello</p>
```

**Advantages**

* Quick styling

**Disadvantages**

* Not reusable
* Hard to maintain

---

## 2. Internal CSS

Defined inside the `<style>` tag in the `<head>` section.

```html
<style>
p {
  color: blue;
}
</style>
```

---

## 3. External CSS

CSS stored in a separate file.

```html
<link rel="stylesheet" href="style.css">
```

style.css

```css
p {
  color: blue;
}
```

**Advantages**

* Reusable
* Clean code
* Easy maintenance

---

# 3. CSS Syntax

Basic syntax:

```css
selector {
  property: value;
}
```

Example:

```css
h1 {
  color: red;
  font-size: 30px;
}
```

Parts:

| Part     | Description          |
| -------- | -------------------- |
| Selector | Target HTML element  |
| Property | Style attribute      |
| Value    | Setting for property |

---

# 4. CSS Selectors

Selectors target HTML elements.

## 1. Element Selector

```css
p {
  color: red;
}
```

Targets all `<p>` elements.

---

## 2. Class Selector

```css
.box {
  color: blue;
}
```

HTML

```html
<p class="box"></p>
```

---

## 3. ID Selector

```css
#header {
  background: black;
}
```

HTML

```html
<div id="header"></div>
```

---

## 4. Universal Selector

```css
* {
  margin: 0;
}
```

Selects all elements.

---

## 5. Group Selector

```css
h1, h2, p {
  color: red;
}
```

---

## 6. Descendant Selector

```css
div p {
  color: blue;
}
```

Targets `p` inside `div`.

---

## 7. Child Selector

```css
div > p {
  color: green;
}
```

Targets **direct children only**.

---

## 8. Attribute Selector

```css
input[type="text"] {
  border: 1px solid black;
}
```

---

# 5. CSS Colors

Ways to define colors:

### Color Names

```css
color: red;
```

### HEX

```css
color: #ff0000;
```

### RGB

```css
color: rgb(255,0,0);
```

### RGBA

```css
color: rgba(255,0,0,0.5);
```

### HSL

```css
color: hsl(0,100%,50%);
```

---

# 6. CSS Units

## Absolute Units

| Unit | Example     |
| ---- | ----------- |
| px   | pixels      |
| cm   | centimeters |
| mm   | millimeters |

Example:

```css
font-size: 16px;
```

---

## Relative Units

| Unit | Description        |
| ---- | ------------------ |
| %    | percentage         |
| em   | relative to parent |
| rem  | relative to root   |
| vw   | viewport width     |
| vh   | viewport height    |

Example:

```css
width: 50%;
```

---

# 7. CSS Box Model

Every element is a **box**.

Structure:

```
Margin
Border
Padding
Content
```

Example:

```css
div {
  margin: 20px;
  border: 2px solid black;
  padding: 10px;
}
```

---

# 8. CSS Background

Properties:

```css
background-color
background-image
background-repeat
background-position
background-size
```

Example:

```css
body {
  background-image: url("image.jpg");
  background-size: cover;
}
```

---

# 9. CSS Borders

Example:

```css
div {
  border: 2px solid black;
}
```

Types:

* solid
* dotted
* dashed
* double
* groove

Border radius:

```css
border-radius: 10px;
```

---

# 10. CSS Text Styling

Properties:

```css
color
text-align
text-decoration
text-transform
line-height
letter-spacing
```

Example:

```css
p {
  text-align: center;
  text-transform: uppercase;
}
```

---

# 11. CSS Fonts

Properties:

```css
font-family
font-size
font-weight
font-style
```

Example:

```css
p {
  font-family: Arial;
  font-size: 18px;
  font-weight: bold;
}
```

---

# 12. CSS Display Property

Controls layout behavior.

Values:

| Value        | Description               |
| ------------ | ------------------------- |
| block        | full width                |
| inline       | no width/height           |
| inline-block | inline but supports width |
| none         | hidden                    |

Example:

```css
div {
  display: block;
}
```

---

# 13. CSS Positioning

Types:

| Type     | Description        |
| -------- | ------------------ |
| static   | default            |
| relative | relative to itself |
| absolute | relative to parent |
| fixed    | fixed on screen    |
| sticky   | hybrid             |

Example:

```css
div {
  position: absolute;
  top: 20px;
  left: 50px;
}
```

---

# 14. Flexbox

Used for **1D layouts**.

Container:

```css
display: flex;
```

Properties:

| Property        | Description          |
| --------------- | -------------------- |
| justify-content | horizontal alignment |
| align-items     | vertical alignment   |
| flex-direction  | row or column        |
| gap             | spacing              |

Example:

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

---

# 15. CSS Grid

Used for **2D layouts**.

Example:

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
```

Example layout:

```css
grid-gap: 20px;
```

---

# 16. CSS Overflow

Controls content overflow.

```css
overflow: hidden;
overflow: scroll;
overflow: auto;
```

---

# 17. CSS Opacity

Controls transparency.

```css
opacity: 0.5;
```

Range:

```
0 → transparent
1 → visible
```

---

# 18. CSS Z-Index

Controls stacking order.

```css
z-index: 10;
```

Higher value appears **on top**.

---

# 19. CSS Transitions

Creates smooth changes.

Example:

```css
button {
  transition: background 0.3s;
}
```

---

# 20. CSS Transform

Transforms elements.

Examples:

```css
transform: rotate(45deg);
transform: scale(1.5);
transform: translateX(50px);
```

---

# 21. CSS Animation

Example:

```css
@keyframes move {
  from {left:0;}
  to {left:200px;}
}

.box {
  animation: move 2s infinite;
}
```

---

# 22. CSS Media Queries (Responsive Design)

Used for responsive websites.

Example:

```css
@media (max-width: 768px) {
  body {
    background: red;
  }
}
```

---

# 23. CSS Pseudo Classes

Used for special states.

Examples:

```css
a:hover
a:active
a:visited
input:focus
```

Example:

```css
button:hover {
  background: blue;
}
```

---

# 24. CSS Pseudo Elements

Style parts of elements.

Examples:

```css
::before
::after
::first-letter
::first-line
```

Example:

```css
p::first-letter {
  font-size: 30px;
}
```

---

# 25. CSS Variables

Reusable values.

```css
:root {
  --main-color: blue;
}

p {
  color: var(--main-color);
}
```

---

# 26. CSS Best Practices

1. Use **external CSS**
2. Follow **consistent naming**
3. Avoid too many **IDs**
4. Use **Flexbox/Grid for layout**
5. Write **responsive CSS**

---

# Advanced CSS Notes

---

# 1. CSS Specificity

Specificity determines **which CSS rule is applied when multiple rules target the same element**.

### Specificity Hierarchy

| Selector Type                    | Weight |
| -------------------------------- | ------ |
| Inline Style                     | 1000   |
| ID Selector                      | 100    |
| Class / Attribute / Pseudo-class | 10     |
| Element / Pseudo-element         | 1      |

Example:

```css
#header {
  color: red;
}

.container p {
  color: blue;
}
```

`#header` has **higher specificity**, so it wins.

---

# 2. CSS Cascade

The **Cascade** determines which style is applied based on:

1. Importance
2. Specificity
3. Source order

Example:

```css
p {
  color: red;
}

p {
  color: blue;
}
```

Result → **blue** (last rule wins).

---

# 3. !important Rule

Forces a rule to override others.

```css
p {
  color: red !important;
}
```

Use **sparingly**, because it breaks maintainability.

---

# 4. Advanced Selectors

### Attribute Selectors

```css
input[type="email"] {
  border: 2px solid blue;
}
```

---

### Starts With

```css
a[href^="https"] {
  color: green;
}
```

---

### Ends With

```css
img[src$=".png"] {
  border: 2px solid red;
}
```

---

### Contains

```css
div[class*="card"] {
  padding: 20px;
}
```

---

# 5. Pseudo Classes (Advanced)

Common advanced pseudo-classes:

| Pseudo Class     | Description                   |
| ---------------- | ----------------------------- |
| `:nth-child()`   | Select element based on index |
| `:nth-of-type()` | Select by type                |
| `:not()`         | Negation selector             |
| `:focus-within`  | Parent when child focused     |
| `:is()`          | Group selectors               |
| `:where()`       | Zero specificity selector     |

Example:

```css
li:nth-child(2) {
  color: red;
}
```

---

# 6. Pseudo Elements (Advanced)

Pseudo-elements style **specific parts of an element**.

Examples:

| Pseudo Element  | Description           |
| --------------- | --------------------- |
| `::before`      | Insert content before |
| `::after`       | Insert content after  |
| `::selection`   | Selected text         |
| `::placeholder` | Input placeholder     |
| `::marker`      | List marker           |

Example:

```css
p::before {
  content: "Note: ";
  color: red;
}
```

---

# 7. CSS Variables (Custom Properties)

Reusable variables inside CSS.

```css
:root {
  --primary-color: #3498db;
  --spacing: 20px;
}

.container {
  color: var(--primary-color);
  padding: var(--spacing);
}
```

Advantages:

* Easy theme changes
* Reusable values
* Maintainable styles

---

# 8. CSS Functions

Common CSS functions:

| Function  | Purpose              |
| --------- | -------------------- |
| `calc()`  | Perform calculations |
| `clamp()` | Responsive sizes     |
| `min()`   | Minimum value        |
| `max()`   | Maximum value        |
| `var()`   | Use variables        |

Example:

```css
width: calc(100% - 50px);
```

---

### clamp()

```css
font-size: clamp(16px, 2vw, 32px);
```

This creates **responsive typography**.

---

# 9. Flexbox (Advanced)

Flexbox is used for **one-dimensional layouts**.

### Flex Container

```css
.container {
  display: flex;
}
```

### Flex Properties

| Property        | Description          |
| --------------- | -------------------- |
| flex-direction  | row / column         |
| flex-wrap       | wrapping             |
| justify-content | horizontal alignment |
| align-items     | vertical alignment   |
| align-content   | multi-line alignment |

Example:

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

---

### Flex Item Properties

```css
flex-grow
flex-shrink
flex-basis
order
align-self
```

Example:

```css
.item {
  flex: 1;
}
```

---

# 10. CSS Grid (Advanced)

Grid is used for **two-dimensional layouts**.

Example:

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

---

### Grid Properties

| Property              | Description  |
| --------------------- | ------------ |
| grid-template-columns | column sizes |
| grid-template-rows    | row sizes    |
| grid-gap              | spacing      |
| grid-area             | define area  |

Example:

```css
grid-template-columns: 200px 1fr 200px;
```

---

### Grid Template Areas

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
}
```

---

# 11. Responsive Design

Responsive design adapts layouts to different devices.

### Breakpoints

Common breakpoints:

| Device  | Width  |
| ------- | ------ |
| Mobile  | <768px |
| Tablet  | 768px  |
| Laptop  | 1024px |
| Desktop | 1200px |

Example:

```css
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

---

# 12. CSS Transitions

Transitions animate property changes.

Example:

```css
button {
  transition: all 0.3s ease;
}

button:hover {
  transform: scale(1.1);
}
```

---

# 13. CSS Transform

Transforms modify element shape or position.

Examples:

```css
transform: rotate(45deg);
transform: scale(1.2);
transform: translateX(100px);
transform: skew(20deg);
```

---

# 14. CSS Animations

Define animations using **keyframes**.

Example:

```css
@keyframes slide {
  0% { transform: translateX(0); }
  100% { transform: translateX(200px); }
}

.box {
  animation: slide 2s infinite;
}
```

---

# 15. CSS Object Fit

Controls how images fit containers.

```css
object-fit: cover;
```

Values:

| Value   | Description    |
| ------- | -------------- |
| cover   | fill container |
| contain | fit inside     |
| fill    | stretch        |

---

# 16. CSS Aspect Ratio

Maintain consistent aspect ratios.

Example:

```css
aspect-ratio: 16/9;
```

Useful for:

* Videos
* Cards
* Images

---

# 17. CSS Filters

Add visual effects.

Example:

```css
filter: blur(5px);
filter: brightness(120%);
filter: grayscale(100%);
```

---

# 18. CSS Clip Path

Creates custom shapes.

Example:

```css
clip-path: circle(50%);
```

Other shapes:

* polygon
* ellipse

---

# 19. CSS Scroll Behavior

Smooth scrolling.

```css
html {
  scroll-behavior: smooth;
}
```

---

# 20. CSS Performance Optimization

Best practices:

1. Avoid deep selectors
2. Minimize `!important`
3. Use classes instead of IDs
4. Reduce large animations
5. Use GPU-friendly properties (`transform`, `opacity`)

---

# 21. Modern CSS Layout Patterns

Common professional patterns:

### Centering

```css
display: flex;
justify-content: center;
align-items: center;
```

---

### Card Layout

```css
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
```

---

### Sticky Header

```css
position: sticky;
top: 0;
```

---

# 22. CSS Methodologies

Used in large projects.

### BEM (Block Element Modifier)

Example:

```css
.card {}
.card__title {}
.card--active {}
```

---

### OOCSS

Object-oriented CSS structure.

---

### Utility-first CSS

Used by frameworks like:

* Tailwind CSS

Example:

```html
<div class="flex items-center justify-center">
```

---

# 23. CSS Preprocessors

Enhance CSS features.

Popular preprocessors:

* Sass
* Less
* Stylus

Example in Sass:

```scss
$primary: blue;

button {
  color: $primary;
}
```

---

# 24. Modern CSS Features

New CSS capabilities used in modern web development:

* Container Queries
* Subgrid
* Logical Properties
* CSS Nesting
* Scroll Snap
* Viewport Units (`svh`, `lvh`, `dvh`)

Example:

```css
.container {
  container-type: inline-size;
}
```

---