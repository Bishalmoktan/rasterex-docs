---
sidebar_position: 2
title: Movement and Interaction
---

## alignCompare
Used to align two documents in an overlay compare. Takes an Array of align objects returned by the GUI_CompareMeasure callback.

### Syntax
```typescript
Syntax: RxCore.alignCompare(array)
```

### Parameters
```typescript
Parameters:
- Array of align objects: Align object = {dist: distance, angle: angle, offset: offset, pwidth: pagewidth}
  offset = {x:xoffset, y:yoffset}

Returns: NA
```

## allowPolygonMove
Turns on the move capability of locked markups like area and polygon.

### Syntax
```typescript
Syntax: RxCore.allowPolygonMove(onoff)
```

### Parameters
```typescript
Parameters:
- onoff: Boolean true = on, false = off

Returns: NA
```