---
sidebar_position: 1
title: Add Methods
---

The main JavaScript object is called RxCore and all following methods are referenced using `RxCore.<Method>`

##  add3DViewAttribute
Adds a custom attribute to a 3D view that is stored with the 3D markup data view.

### Syntax
```typescript
Syntax: RxCore.add3DViewAttribute(atName, atValue, viewname)
```
### Parameters
```typescript
Parameters:
- atName: string - Name of the custom attribute
- atValue: string - Value of the custom attribute
- viewname: string - Name of the view. The view name can be extracted from any 3D annotation as the name property of the annotation.

Returns: NA
```

### Example
```typescript
Example:
RxCore.add3DViewAttribute("description", "my description", annotitem.name);
```

##  addFill
To populate various fill styles to use with CAD polygons.

### Syntax
```typescript
Syntax: RxCore.addFill(type, name, image, tilesize, color, ledgend_description)
```
### Parameters
```typescript
Parameters:
- type: string - Should be 'hatch' or 'color'
- name: string - Name of the fill entry to be used when applying the fill
- image: Html image or null - For hatch the image object used as fill repeat image
- tilesize: object - {w: number, h: number} size of the hatch image in pixels
- color: Html color - Color of the hatch or color fill
- ledgend_description: string - Description of the fill to be used in a ledgend displayed with the drawing

Returns: NA
```
### Example
```typescript

Example:
// Red fill color with 0.5 transparency
RxCore.addFill('color', 'transpred', null, null, 'rgba(255,0,0,0.5)', 'BTA');

// Adding a hatch using an image of 16x16 pixels
RxCore.addFill('hatch', 'diagonal-forward', image,{w:16, h:16}, 
'rgba(255,0,0,0.5)', 'Non usable space');
```

## addGltftoDoc
Add a model to an already open 3D model. Used to add separate type of 3D entities to a 3D model like structure and site.

### Syntax
```typescript
Syntax: RxCore.addGltftoDoc(URL)
```

### Parameters
```typescript
Parameters:
- URL: URL or path to an IFC file to add to the currently open 3D model. If path it must be relative to the server.

Returns: NA
```


## addHoverforBlock
Mark a vector 2D polygon with a different color. Used in combination with GUI_2DBlockInfoPos for mouse over indication. Use clearHover to remove the marking.

### Syntax
```typescript
Syntax: RxCore.addHoverforBlock(blockindx, color)
```

### Parameters
```typescript
Parameters:
- blockindx: Block index returned by GUI_2DBlockInfoPos
- color: Highlight color to use on 2D vector polygon

Returns: NA
```

##  addMarkup
Add one or more markup entities using XML encoded text.

### Syntax
```typescript
Syntax: RxCore.addMarkup(markupxml)
```

### Parameters
```typescript
Parameters:
- markupxml: String in xml format that holds tags in accordance with RxView360 xml based markup format.

Returns: NA
```



