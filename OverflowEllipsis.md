# SPAN (inline) inside DIV prevents text-overflow:ellipsis

##  SPAN (inline) will never overflow
At least that's how the W3 spec states this gets triggered.
https://stackoverflow.com/questions/10217915/span-inside-div-prevents-text-overflowellipsis

https://drafts.csswg.org/css-ui-3/#text-overflow

Applies to:	block containers

# Hover To View Hidden Text Overflow
https://www.willmaster.com/library/web-development/hover-to-view-hidden-text-overflow.php

```css
white-space: nowrap; /*keeps all text on one line*/
overflow: hidden; /*to clip any text that extends past the right side of the container.*/
text-overflow :ellipsis; /*to print an elipsis where some of the text is clipped.*/
/*Use the overflow:visible; CSS declaration for the class' :hover selector.*/
```

# expand the content to its full length on mouseover.
https://stackoverflow.com/a/33422695
https://stackoverflow.com/questions/5474871/html-how-can-i-show-tooltip-only-when-ellipsis-is-activated
