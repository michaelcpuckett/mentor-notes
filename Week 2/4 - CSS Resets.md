# CSS Resets

## Overriding Browser Styles

Web browsers apply default styles to built-in elements. Web developers tend to override some of these defaults to make development easier.

```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  -webkit‑text‑size‑adjust: 100%;
}

img {
  max-width: 100%;
}
```

You can use the Web Inspector to see the browser's default styles.

```css
button {
  padding: 1px 6px;
  /* ... */
  /* See inspector for all properties. */
}
```

You can override the defaults, or remove them with the `unset` keyword.

Here, with `unset`, all <button>s will appear like <div>s:

```css
button {
  background: unset;
  border: unset;
  color: unset;
  font: unset;
  padding: unset;
}
```
