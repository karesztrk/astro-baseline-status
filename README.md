# Astro Baseline Status

A widget displaying Baseline status of a web feature based on https://github.com/web-platform-dx/web-features data.

![Default browser icons rendered](./docs/default_icons.png "Default browser icons")

![Custom browser icons can be added](./docs/custom_icons.png "Custom browser icons")

## How to use

Import the Astro component.
Optionally import your browser images. If omitting, the default images will be used.

```jsx
---
import BaselineStatus from "astro-baseline-status";
import Chrome from "./assets/Chrome.svg";
import Edge from "./assets/Edge.svg";
import Firefox from "./assets/Firefox.svg";
import Safari from "./assets/Safari.svg";
---
<BaselineStatus feature-id={feature}>
  <svg
    slot="chrome"
    role="img"
    aria-label={...}
    src={...}
    viewBox={`0 0 ...`}
  />
  <!-- <svg -->
  <!--   slot="edge" -->
  <!--   role="img" -->
  <!--   aria-label={...} -->
  <!--   src={...} -->
  <!--   viewBox={`0 0 ...`} -->
  <!-- /> -->
  <!-- <svg -->
  <!--   slot="firefox" -->
  <!--   role="img" -->
  <!--   aria-label={...} -->
  <!--   src={...} -->
  <!--   viewBox={`0 0 ...`} -->
  <!-- /> -->
  <!-- <svg -->
  <!--   slot="safari" -->
  <!--   role="img" -->
  <!--   aria-label={...} -->
  <!--   src={...} -->
  <!--   viewBox={`0 0 ...`} -->
  <!-- /> -->
</BaselineStatus>
```

## Advantages

- 💅 An Bring your own style
- 📷 An Use your own images
