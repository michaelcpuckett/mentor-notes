# Responsive Web Design

## History lesson

The core idea behind Responsive Web Design is using the same HTML at different screen sizes, such as mobile devices and widescreen desktops.

This technique has been an industry best practice for over a decade because it avoids the need to create separate HTML for different screen sizes.

In the past, some websites would create a “mobile version” that would be entirely different from the regular site.

This caused two main issues:

1. The amount of work needed to maintain two separate websites.
2. Users could not always find the same content or perform the same actions when they switched between mobile and desktop. Mobile versions were rarely at “feature parity” with the regular site.

## The fluid nature of web content

In an HTML document without CSS, browsers automatically wrap lines of text and allow for scrolling, based on the available screen space. If the user changes the window size, the browser will automatically readjust to fit.

## Static representations of web layouts are always misleading

With more complex layouts, designers must make decisions about how the content should adjust to fit at different screen sizes.

At least two design mockups are needed to build a web page — horizontal (desktop) and vertical (mobile).

Even with two mockups, designers cannot possibly foresee every possible screen size, combined with other factors like zoom level and system settings. This means deferring to the browser’s natural behavior whenever possible.

Designers must also decide whether the layout will be Adaptive or fully Responsive.

1. Adaptive Layouts
   - Have fixed widths at different breakpoints
2. Responsive Layouts
   - No fixed widths, mostly percentage-based widths

## Mobile considerations

On mobile, there are a few differences from desktop:

- Small overall area (”real estate”)
  - Hamburger menus hide navigation behind a button
- Narrow screen
  - Most things are 100% width, not in columns
- Finger as pointer
  - Not as precise, so the element sizes should be at least 48px x 48px
- Data plans and possibly poor data connection
  - Don’t send unnecessary desktop styles until needed
- The viewport must be set in the HTML

```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
```
