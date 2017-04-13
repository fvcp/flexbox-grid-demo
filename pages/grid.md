---
title: 'Grid'
template: '_index.html'
---

> CSS Grid Layout introduces a two-dimensional grid system to CSS. Grids can be used to lay out major page area or small user interface elements.
> 
> — [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout#The_fr_Unit "Basic concepts of grid layout - CSS | MDN")

## What the “fr”?

The new `fr` unit is a “fraction of the available space in the grid container”.

## Parent Container

```
.parent {
    // Define the container as a grid. Establish grid context for children
    display: grid;

    // Establish grid
    grid-template {
        grid-template-rows:
        grid-template-columns:
        grid-template-areas:
    }

    // Set the grid gap (gutter) between grid elements (NOT AROUND THE GRID)
    grid-gap {
        grid-column-gap:
        grid-row-gap:
    }

    // Align items along row axis
    justify-items:

    // Align items along column axis
    align-items:
}
```

## Child Item
```
.child {
    // Dictate the grid item location
    grid-column {
        grid-column-start: line span
        grid-column-end:
    }

    grid-row {
        grid-row-start: row span
        grid-row-end:
    }

    // Specify a named grid template area
    grid-area: name
    
    // Align content along row axis
    justify-self:

    // Align content along column axis
    align-self:
}
```
