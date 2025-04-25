# nebo.css

Negative border radius made easy

> Nebo.css is a pure CSS solution that allows you to add a “convex” or “concave” puzzle angle to elements without
> SVG and JavaScript. Everything is controlled via custom CSS variables.

## Преимущества

- ⚡ CSS only — no images or scripts;
- 🎛 Flexible customization via variables:
  - `--nb-r` - radius of main rounding;
  - `--nb-w` - width of protrusion/cutout;
  - `--nb-h` - height of protrusion/cutout;
- 🧩 4 modifiers for angle positioning: `.nebo--tl`, `.nebo--tr`, `.nebo--bl`, `.nebo--br`;
  ![Example of using modifiers](assets/examples.jpg)
- 🖼 Supports any backgrounds (solid colors, gradients, images);
- 🕸 Modern browser support (mask-image).

## Example of use

```html

<div class="card nebo nebo--br">
  Card Content
</div>
```

```css
.card {
  --nb-r: 24px; /* radius of curvature  */
  --nb-w: 28px; /* protrusion width */
  --nb-h: 28px; /* protrusion height */
  background: linear-gradient(135deg, #b98bff, #6244d6);
  padding: 2rem;
  color: #fff;
  font: 16px/1.4 "Inter", sans-serif;
}
```

Combine modifiers to get a four-piece puzzle:

```html

<div class="grid">
  <div class="nebo nebo--tl"></div>
  <div class="nebo nebo--tr"></div>
  <div class="nebo nebo--bl"></div>
  <div class="nebo nebo--br"></div>
</div>
```

## Browser support

| Browser | Version | 
|---------|---------|
| Chrome  | 60+     |
| Edge    | 79+     |
| Firefox | 53+     |
| Safari  | 14+     |
