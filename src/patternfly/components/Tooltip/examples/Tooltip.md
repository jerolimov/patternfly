---
id: Tooltip
section: components
cssPrefix: pf-c-tooltip
---

## Examples
### Top
```hbs
{{#> tooltip tooltip--modifier="pf-m-top"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-top-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

### Right
```hbs
{{#> tooltip tooltip--modifier="pf-m-right"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-right-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

### Bottom
```hbs
{{#> tooltip tooltip--modifier="pf-m-bottom"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-bottom-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

### Left
```hbs
{{#> tooltip tooltip--modifier="pf-m-left"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-left-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

### Left with top and bottom positions
```hbs
{{#> tooltip tooltip--modifier="pf-m-left-top"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-left-top-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
<br />
{{#> tooltip tooltip--modifier="pf-m-left-bottom"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-left-bottom-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

### Bottom with left and right positions
```hbs
{{#> tooltip tooltip--modifier="pf-m-bottom-left"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-bottom-left-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
<br />
{{#> tooltip tooltip--modifier="pf-m-bottom-right"}}
  {{#> tooltip-content tooltip-content--attribute='id="tooltip-bottom-right-content"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

### Left aligned text
```hbs
{{#> tooltip tooltip--modifier="pf-m-top"}}
  {{#> tooltip-content tooltip-content--modifier="pf-m-text-align-left" tooltip-content--attribute='id="tooltip-text-align-left-example"'}}
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam id feugiat augue, nec fringilla turpis.
  {{/tooltip-content}}
{{/tooltip}}
```

## Documentation
### Overview
A tooltip is used to provide contextual information for another component on hover.  The tooltip itself is made up of two elements: arrow and content. One of the directional modifiers (`.pf-m-left`, `.pf-m-top`, etc.) is required on the tooltip component.

### Usage
| Class | Applied to | Outcome |
| -- | -- | -- |
| `.pf-c-tooltip` | `<div>` |  Creates a tooltip. Always use with a modifier class that positions the tooltip relative to the element it describes. **Required**|
| `.pf-c-tooltip__arrow` | `<div>` |  Creates an arrow pointing towards the element the tooltip describes. **Required** |
| `.pf-c-tooltip__content` | `<div>` |  Creates the body of the tooltip. **Required** |
| `.pf-m-left{-top/bottom}` | `.pf-c-tooltip` | Positions the tooltip to the left (or left top/left bottom) of the element. |
| `.pf-m-right{-top/bottom}` | `.pf-c-tooltip` | Positions the tooltip to the right (or right top/right bottom) of the element. |
| `.pf-m-top{-left/right}` | `.pf-c-tooltip` | Positions the tooltip to the top (or top left/top right) of the element. |
| `.pf-m-bottom{-left/right}` | `.pf-c-tooltip` | Positions the tooltip to the bottom (or bottom left/bottom right) of the element. |
| `.pf-m-text-align-left` | `.pf-c-tooltip__content` | Modifies tooltip content to text align left. |
