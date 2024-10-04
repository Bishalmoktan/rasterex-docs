---
sidebar_position: 3
title: Block and Sizing
---

## appendCustomBlockAttribute
For vector files with blocks you can add custom attributes that can be displayed when selecting a block.

### Syntax
```typescript
Syntax: RxCore.appendCustomBlockAttribute(blockid, name, value)
```

### Parameters
```typescript
Parameters:
- blockid: Unique ID of the block that attributes should be added to
- name: Name of the added attribute
- value: Value of the added attribute

Returns: NA
```

## applyAngleLength
When using a markup drawing tool that supports setting angle and length of a line, this can be used to override the mouse input and set angle and length using parameters. Values are in degrees and current active measurement unit. Works in combination with GUI_markupDrawParams event callback that returns the values set or GUI_markupParamError that will be called if values exceed drawing boundaries.

### Syntax
```typescript
Syntax: RxCore.applyAngleLength(angle, length, bAdvance)
```

### Parameters
```typescript
Parameters:
- angle: Direction to draw the line in current active measurement unit. Ex mm.
- length: Length of the line in current active measurement unit. Ex mm.
- bAdvance: If enabled will continue segments and this is how the active segment will be the next two points. If false the active segment will remain the current segment.

Returns: NA
```