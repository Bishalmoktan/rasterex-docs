Starts the search for matching texts and returns the text rectangles in a callback.

### Syntax

```typescript
RxCore.getTextRects(searchexpr, casesensitive)
```

### Parameters

- `searchexpr`: **string** — The string to search for.
- `casesensitive`: **boolean** — If `true`, the search is case-sensitive.

### Returns

- **NA** — This method does not return a value.

### Example

```typescript
RxCore.getTextRects("Rasterex", false);
// Returns all rectangles for the word "Rasterex" regardless of case.
```

### Callbacks

- **RxCore.GUI_MathcesRectsPage**
- **RxCore.GUI_NumMathcesRect**