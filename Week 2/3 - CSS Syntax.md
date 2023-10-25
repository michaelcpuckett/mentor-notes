# CSS Syntax

## Anatomy of a CSS rule

HTML has elements. CSS has rules.

CSS rules have 3 parts:

- Selector: Targets one or more HTML elements.
- Property: A known CSS keyword that controls some aspect of the style
- Value: What the property is being set to

```css
/* <selector></selector> */

selector {
  property: value;
}
```

## Targeting HTML elements for styling

By HTML element name:

```css
/* <michaels-element>Hello world!</michaels-element> */

michaels-element {
  background-color: red;
}

h1 {
  font-size: 16px;
}
```

With a class:

```css
/* <div class=”michaels-class”></div> */

.michaels-class {
  background-color: red;
}
```

## Overrides

If there are duplicates, the last one down will apply:

```css
michaels-element {
  font-size: 64px;
}

michaels-element {
  font-size: 24px;
}
```

Selectors are be weighted (by “specificity”) when you combine them:

```css
div.michaels-class {
  background-color: green;
}

.michaels-class {
  background-color: red;
}
```

## Variables/Custom Properties

Define custom properties at the top level:

```css
:root {
  --my-custom-property: 12px;
}
```

Use multiple times with the `var()` keyword:

```css
p {
  margin-top: var(--my-custom-property);
}

img {
  padding: var(--my-custom-property);
}
```

Use in calculations with the `calc()` keyword:

```css
h1 {
  font-size: calc(var(--my-custom-property) * 2);
}
```
