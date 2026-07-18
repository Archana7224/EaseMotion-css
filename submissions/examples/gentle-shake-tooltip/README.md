# CSS Micro Shake Popover

A lightweight, responsive, and accessible popover component built entirely with **HTML and CSS**.

## Features

- ✅ Pure CSS
- ✅ No JavaScript
- ✅ Micro Shake Animation
- ✅ Responsive Layout
- ✅ Accessibility Friendly
- ✅ Keyboard Navigation
- ✅ CSS Custom Properties
- ✅ Dark Mode Support
- ✅ Modern SaaS Styling

---

## Demo Examples

This demo includes:

1. Primary Button Popover
2. Info Icon Popover
3. Strong Shake Variant
4. Dark Theme Example

---

## Folder Structure

```
micro-shake-popover/
│
├── index.html
├── style.css
└── README.md
```

---

## CSS Variables

```css
--shake-distance
--shake-duration
--shake-easing

--popover-bg-color
--popover-text-color
--popover-shadow
--popover-border-radius
--popover-padding
```

---

## Accessibility

- Uses `role="tooltip"`
- Uses `aria-describedby`
- Keyboard accessible
- Visible focus styles
- Supports `prefers-reduced-motion`

---

## Responsive

Optimized for:

- Desktop
- Tablet
- Mobile (<768px)

---

## Browser Support

- Chrome
- Firefox
- Safari
- Edge

---

## Customization

### Stronger Shake

```css
.popover-wrapper{
    --shake-distance:6px;
}
```

### Slower Animation

```css
.popover-wrapper{
    --shake-duration:1s;
}
```

### Dark Theme

```css
.popover-wrapper{
    --popover-bg-color:#1f2937;
    --popover-text-color:#f3f4f6;
}
```

---

## Animation

```css
@keyframes microShake {
  0%,100%{
    transform:translateX(0);
  }

  25%{
    transform:translateX(var(--shake-distance));
  }

  50%{
    transform:translateX(calc(var(--shake-distance) * -1));
  }

  75%{
    transform:translateX(var(--shake-distance));
  }
}
```

---

## License

MIT