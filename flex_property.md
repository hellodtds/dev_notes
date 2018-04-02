## Flex

The flex property is a sub-property of the Flexible Box Layout module.

This is the shorthand for flex-grow, flex-shrink and flex-basis. The second and third parameters (flex-shrink and flex-basis) are optional.

[More on Flex](https://css-tricks.com/almanac/properties/f/flex/)

## Flex-grow

The flex-grow property is a sub-property of the Flexible Box Layout module.

IT defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.

For example, if all items have flex-grow set to 1, every child will set to an equal size inside the container. If you were to give one of the children a value of 2, that child would take up twice as much space as the others.

[More on flex-grow](https://css-tricks.com/almanac/properties/f/flex-grow/)

## Flex-shrink

The flex-shrink property is a sub-property of the Flexible Box Layout module.

It specifies the "flex shrink factor", which determines how much the flex item will shrink relative to the rest of the flex items in the flex container when there isn't enough space on the row.

When omitted, it is set to 1 and the flex shrink factor is multiplied by the flex basis when distributing negative space.

[More on Flex-shrink](https://css-tricks.com/almanac/properties/f/flex-shrink/)

## Flex-basis

The flex-basis property is a sub-property of the Flexible Box Layout module.

It specifies the initial size of the flex item, before any available space is distributed according to the flex factors. When omitted from the flex shorthand, its specified value is the length zero.

A flex-basis value set to auto sizes the element according to its size property (which can itself be the keyword auto, which sizes the element based on its contents).

[More on Flex-basis](https://css-tricks.com/almanac/properties/f/flex-basis/)
