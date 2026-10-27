# Pixel Studio — HTML & CSS Practice

## Project Overview
Built a simple digital agency landing page featuring two service cards:
- Web Design
- Brand Identity

The project helped me practise HTML structure, CSS styling, layout, spacing, and responsive design.

## What I Learned

### 1. HTML Structure
- Use semantic elements such as `<header>` and `<footer>` to organise page content.
- Use `<div>` to group related elements.
- Keep independent components as sibling elements when they should be styled separately.
- The `<img>` element is a void element and does not need a closing tag.
- Use descriptive `alt` text for images.

### 2. CSS Classes
An element can have multiple classes:

```html
<div class="left card">Content</div>
```

This element has two classes: `left` and `card`.

```css
.left.card {
  /* Targets an element with both classes */
}
```

```css
.left .card {
  /* Targets a .card descendant inside a .left element */
}
```

The space between selectors changes their meaning.

### 3. CSS Cascade
When two declarations have equal specificity and both apply, the later declaration wins.

For example:

```css
.card {
  width: 45%;
}

.card {
  width: 100%;
}
```

The computed width is `100%`, assuming no other conflicting rules.

### 4. Responsive Design
Media queries apply styles when specified viewport conditions are met.

```css
.card {
  width: 45%;
}

@media (max-width: 680px) {
  .card {
    width: 100%;
  }
}
```

- Above 680px: the card width is 45% of its containing block.
- At or below 680px: the card width is 100% of its containing block.

A media query must have matching opening and closing braces.

### 5. Spacing with Margins
Margins control the space outside an element's border.

```css
.logo {
  margin-bottom: 10px;
}

h1 {
  margin-top: 10px;
}
```

These properties help adjust the distance between the logo and the heading.

The final spacing also depends on the elements' default margins and layout.

### 6. Typography
```css
h1 {
  font-size: 5rem;
}

@media (max-width: 680px) {
  h1 {
    font-size: 3.5rem;
  }
}
```

This provides different heading sizes for desktop and smaller screens.

## Debugging Lessons
- Check whether media queries are present and correctly closed.
- Remember that CSS rules can override earlier declarations.
- Inspect the element's computed styles when a change does not produce the expected result.
- Test the page at desktop and mobile viewport widths.
- Compare the browser output with the intended layout.

## What I Need to Practise Next
1. Writing HTML without basic syntax errors.
2. Understanding CSS specificity and the cascade.
3. Building two-column layouts and stacking them on mobile.
4. Adjusting spacing deliberately rather than guessing.
5. Debugging with browser developer tools.
6. Rebuilding a similar page without copying the original code.

## Key Takeaway
Building the page helped me identify the difference between recognising HTML and CSS concepts and applying them independently. My next goal is to strengthen the fundamentals through small projects and deliberate debugging practice.
