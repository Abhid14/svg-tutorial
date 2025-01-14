---
day: 13
title: How to Draw a Bell with SVG
component: Bell
description: In this example we draw a Bell with SVG and practice drawing complex paths that combine quadratic and cubic bézier curves.
previous:
  title: Cubic Bézier
  link: cubic-bezier
next:
  title: How to Draw an Arc with SVG
  link: arc
---

Let’s have another example with cubic and quadratic beziers.

Here the bottom of this bell is defined with straight lines.

<div class="grid-200">

<svg width="200" height="200" viewBox="-100 -100 200 200" stroke="black" stroke-width="2">
  <path
      d="
        M -50 40
        L -50 50
        L 50 50
        L 50 40"
      fill="#FDEA96"
    />
</svg>

<!-- prettier-ignore -->
```html
<svg 
  width="200"
  height="200"
  viewBox="-100 -100 200 200"
  stroke="black"
  stroke-width="2"
>
  <path
    d="
      M -50 40
      L -50 50
      L 50 50
      L 50 40"
    fill="#FDEA96"
  />
</svg>
```

</div>

Then a quadratic Beziers starts the bell cloak.

<div class="grid-200">

<svg width="200" height="200" viewBox="-100 -100 200 200" stroke="black" stroke-width="2">
  <path
    d="
      M -50 40
      L -50 50
      L 50 50
      L 50 40
      Q 40 40 40 10"
    fill="#FDEA96"
  />
  <circle 
    cx="40"
    cy="40"
    r="2" 
    stroke="none"
    fill="red"
  />
</svg>

<!-- prettier-ignore -->
```html
<svg 
  width="200"
  height="200"
  viewBox="-100 -100 200 200"
  stroke="black"
  stroke-width="2"
>
  <path
    d="
      M -50 40
      L -50 50
      L 50 50
      L 50 40
      Q 40 40 40 10"
    fill="#FDEA96"
  />
</svg>
```

</div>

Then the line is continued with a cubic Bezier to form the top of the bell.

<div class="grid-200">

<svg width="200" height="200" viewBox="-100 -100 200 200" stroke="black" stroke-width="2">
  <path
    d="
      M -50 40
      L -50 50
      L 50 50
      L 50 40
      Q 40 40 40 10
      C 40 -60 -40 -60 -40 10"
    fill="#FDEA96"
  />
  <circle 
    cx="-40"
    cy="-60"
    r="2" 
    stroke="none"
    fill="red"
  />
  <circle 
    cx="40"
    cy="-60"
    r="2" 
    stroke="none"
    fill="red"
  />
</svg>

<!-- prettier-ignore -->
```html
<svg 
  width="200"
  height="200"
  viewBox="-100 -100 200 200"
  stroke="black"
  stroke-width="2"
>
  <path
    d="
      M -50 40
      L -50 50
      L 50 50
      L 50 40
      Q 40 40 40 10
      C 40 -60 -40 -60 -40 10"
    fill="#FDEA96"
  />
</svg>
```

</div>

Then we reach the bottom part with another quadratic bezier that mirrors the previous one.

<div class="grid-200">

<svg width="200" height="200" viewBox="-100 -100 200 200" stroke="black" stroke-width="2">
  <path
    d="
      M -50 40
      L -50 50
      L 50 50
      L 50 40
      Q 40 40 40 10
      C 40 -60 -40 -60 -40 10
      Q -40 40 -50 40"
    fill="#FDEA96"
  />
  <circle 
    cx="-40"
    cy="40"
    r="2" 
    stroke="none"
    fill="red"
  />
</svg>

<!-- prettier-ignore -->
```html
<svg 
  width="200"
  height="200"
  viewBox="-100 -100 200 200"
  stroke="black"
  stroke-width="2"
>
  <path
      d="
        M -50 40
        L -50 50
        L 50 50
        L 50 40
        Q 40 40 40 10
        C 40 -60 -40 -60 -40 10
        Q -40 40 -50 40"
      fill="#FDEA96"
    />
</svg>
```

</div>

We finish the bell, by adding two circles for the bell-clapper, and the hanger.

<div class="code-flex">

```html
<svg width="200" height="200" viewBox="-100 -100 200 200">
  <g stroke="black" stroke-width="2">
    <circle cx="0" cy="-45" r="7" fill="#4F6D7A" />
    <circle cx="0" cy="50" r="10" fill="#F79257" />
    <path
      d="
        M -50 40
        L -50 50
        L 50 50
        L 50 40
        Q 40 40 40 10
        C 40 -60 -40 -60 -40 10
        Q -40 40 -50 40"
      fill="#FDEA96"
    />
  </g>
</svg>
```

</div>
