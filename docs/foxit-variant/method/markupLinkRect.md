Creates a markup with a link based on a text rectangle from the `RxCore.GUI_MathcesRectsPage` or `RxCore.GUI_NumMathcesRect` callbacks.

### Syntax

```typescript
RxCore.markupLinkRect(usemarker, rectangle, page, linkurl, padding)
```

### Parameters

- `usemarker`: **boolean** — Set to `true` to create a marker rectangle, or `false` to create an outline rectangle.
- `rectangle`: **object** — Defines the rectangle's start point and dimensions:

```typescript
rectangle = { x: number, y: number, w: number, h: number };
```

- `page`: **number** — The 0-indexed page number for the markup.
- `linkurl`: **string** — The URL to which the link directs.
- `padding` (optional): **object** — Specifies additional space around the markup:

```typescript
padding = { top: number, left: number, right: number, bottom: number };
```

### Returns

- **NA** — This method does not return a value.