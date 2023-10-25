# CSS Media Queries

## Targeting different screen widths

The point at which the layout switches from one design to another is called a breakpoint.

```css
/* Mobile */
body {
  font-size: 16px;
}

/* Tablet */
@media (min-width: 800px) {
  body {
    font-size: 18px;
  }
}

/* Wide screen */
@media (min-width: 12000px) {
  body {
    font-size: 20px;
  }
}
```

Building mobile-first means mobile styles are not in a media query.

## Handling user preferences

When possible, design to fit the user’s system preferences.

Some users prefer darker colors on their screen due to light fatigue or other reasons.

Accomodate those users whenever possible by providing an alternate design.

```css
body {
  background-color: lightyellow;
}

@media (prefers-color-scheme: dark) {
  body {
    background-color: darkpurple;
  }
}
```

Some system preferences define accessibility settings.

Animations should always be gated so as not to disturb those with motion disorders.

```css
@media (prefers-reduced-motion: no-preference) {
  .spinner {
    animation: spin-around-the-page 2s;
  }
}
```
