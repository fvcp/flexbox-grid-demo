---
title: 'Flexbox'
template: '_flex.html'
---

> CSS Flexible Box Layout is a module of CSS that defines a CSS box model optimized for user interface design. In the flex layout model, the children of a flex container can be laid out in any direction, and can “flex” their sizes, either growing to fill unused space or shrinking to avoid overflowing the parent.
> 
> — [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout "CSS Flexible Box Layout - CSS | MDN")

## Parent Container

```
.parent {
    // Define the container as a flex container. All direct children are flex items/
    display: flex;

    // Establish the main axis
    flex-direction: column/row

    // Flexbox wants to stay in line, you can tell it to wrap
    flex-wrap: nowrap;

    // Define alignment along main axis (flex-direction) and sitribute free space.
    justify-content: start;

    // Set alignment along the cross axis (the opposite of flex-direction)
    align-items: stretch;
}
```

## Child Item
```
.child {
    // Dictate the display order if it differs from source order
    order: 1;
    
    flex {
        // If necessary, a flex item can grow to take up remaining space
        flex-grow: 2; (will take up twice the extra space of a flex-grow: 1)

        // If necessary, a flex item can shrink
        flex-shrink: 1;

        // Set the default size of a flex item
        flex-basis: 20%/5em/20px;
    }

    // Override the default alignment set by the parent
    align-self: start;
}
```
