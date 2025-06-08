# CSS Cheatsheet by Parichehr Abedzadeh

> A comprehensive CSS reference for developers. Includes syntax, examples, and best practices.

GitHub: [https://github.com/parichabd](https://github.com/parichabd)

---

## Table of Contents
- [CSS Types](#css-types)
- [Selector Types](#selector-types)
- [Units in CSS](#units-in-css)
- [Box Model](#box-model)
- [Display and Positioning](#display-and-positioning)
- [Flexbox](#flexbox)
- [Grid](#grid)
- [Text & Font Styling](#text--font-styling)
- [Backgrounds & Gradients](#backgrounds--gradients)
- [Media Queries](#media-queries)
- [Transitions & Animations](#transitions--animations)
- [Filters](#filters)
- [Variables](#variables)
- [Useful Resources](#useful-resources)

---

## CSS Types

```html
<!-- Inline -->
<p style="color: red;">Inline CSS</p>

<!-- Internal -->
<style>
p { color: blue; }
</style>

<!-- External -->
<link rel="stylesheet" href="styles.css">
```

**Priority:** Inline > Internal > External (but external is preferred for maintainability).

---

## Selector Types

```css
*               /* Universal */
p               /* Type */
.box            /* Class */
#main           /* ID */
div span        /* Descendant */
div > span      /* Child */
div + span      /* Adjacent sibling */
div ~ span      /* General sibling */
a[href]         /* Attribute */
a:hover         /* Pseudo-class */
p::first-line   /* Pseudo-element */
```

---

## Units in CSS

| Unit   | Relative To           | Example             | Use Case                      |
|--------|------------------------|---------------------|-------------------------------|
| px     | Fixed                  | width: 100px        | Precise spacing               |
| em     | Parent font-size       | padding: 2em        | Scalable spacing              |
| rem    | Root font-size         | font-size: 1.5rem   | Consistent scaling            |
| %      | Parent element         | width: 50%          | Responsive layouts            |
| vw/vh  | Viewport               | height: 100vh       | Full-screen sections          |

---

## Box Model

```css
div {
  padding: 10px;
  border: 2px solid black;
  margin: 20px;
  box-sizing: border-box;
}
```

---

## Display and Positioning

- `display: block | inline | inline-block | none`
- `position: static | relative | absolute | fixed | sticky`
- `visibility: hidden` vs `opacity: 0` vs `display: none`

---

## Flexbox

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 10px;
}
```

---

## Grid

```css
.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}
```

---

## Text & Font Styling

```css
h1 {
  color: #333;
  font-family: 'Arial', sans-serif;
  font-size: 2rem;
  text-align: center;
  line-height: 1.5;
  text-transform: uppercase;
}
```

---

## Backgrounds & Gradients

```css
.section {
  background: linear-gradient(to right, #ff6a00, #ee0979);
  background-repeat: no-repeat;
  background-size: cover;
}
```

---

## Media Queries

```css
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
```

---

## Transitions & Animations

```css
.button {
  transition: background-color 0.3s ease;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

.box {
  animation: fadeIn 2s ease-in-out;
}
```

---

## Filters

```css
img {
  filter: grayscale(100%) blur(2px);
}
```

---

## Variables

```css
:root {
  --main-color: #3498db;
}

h2 {
  color: var(--main-color);
}
```

---

## Useful Resources

- [CSS Tricks](https://css-tricks.com/)
- [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [Google Fonts](https://fonts.google.com/)
- [CSS Gradient Generator](https://cssgradient.io/)
- [Font Awesome](https://fontawesome.com/)

---

**Author:** Parichehr Abedzadeh  
GitHub: [github.com/parichabd](https://github.com/parichabd)
