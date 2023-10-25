# Browser Support

## Where does CSS come from?

CSS is changing all the time.

Over the years, new CSS has given web developers new powers: media queries, Photoshop-style filters, animations, and more.

New CSS properties and syntax are introduced through an open process that includes the companies that design and code web browser engines:

Chromium

- Chrome (Google)
- Edge (Microsoft)

WebKit

- Safari (Apple)

Gecko

- Firefox (Mozilla)

Google, Microsoft, Apple, and Mozilla listen to developer input and decide together whether to make and implement changes to the CSS specification.

## Cross-Browser Testing

Unfortunately, the browsers may have slight differences in their imlementations.

It's important to check the apperance and functionality of a web page in all browsers, because there might be differences or even bugs.

## Automatic Updates

Browsers used to require users to download new versions, or were tied to operating systems that updated every few years.

This caused problems because browsers were adopting new CSS at a very slow rate.

Now all browsers are "evergreen" one-time downloads that update themselves automatically, or are tied to more frequent operating system updates.

There are some cases where older browsers need to be considered, but now it's easier to assume that most users are on the latest technology.

When you discover new CSS, you can check the website caniuse.com to see which browsers have implemented it.

## Example: CSS Nesting

This year, a new CSS syntax was introduced into browsers.

To target these elements:

```html
<div class="a">
  Red
  <div class="b">
    Green
    <div class="c">Blue</div>
  </div>
</div>
```

Old Style:

```css
.a {
  color: red;
}

.a .b {
  color: green;
}

.a .b .c {
  color: blue;
}
```

Since 2023:

```css
.a {
  color: red;

  .b {
    color: green;

    .c {
      color: blue;
    }
  }
}
```

For browser support, see: https://caniuse.com/css-nesting
