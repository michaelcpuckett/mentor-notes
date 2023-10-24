# CSS Resets

# Overriding Browser Styles

Web browsers apply default styles to build-in elements. Web developers tend to override some of these defaults to make development easier.

```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  -webkit‑text‑size‑adjust: 100%
}

img {
  max-width: 100%;
}
```