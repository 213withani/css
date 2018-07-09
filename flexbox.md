# Flexbox Tutorial (CSS): Real Layout Examples
https://www.youtube.com/watch?v=k32voqQhODc

##  Example # 1: Have input fill out rest of line

Opens new ways of sizing the children elements under container flex.

```display: flex;```

Fills up remainder space if this is the only element with flex 1, otw it shares space with other flex:#

```flex:1```

##  Example # 2: Better understand flex:1
### Three Column Layout

```display: flex;``` This will make divs, block elements, sit side by side. Will also set width based on content.
 
 Three equal width column: Set each div/column to ```flex:1```. If you want an element the same size as its siblings then set all of them to the same flex number, baseline starts at 1. We can use bigger numbers in relation to one to create different sizes.
 
 Not all elements must have ```flex:1```. If elements don't have ```flex:1``` they will keep their auto size.

Ordering of content can be set using order property i.e. ```order:1```

##  Example # 3: Adding Margins
Margins in btwn columns can be set using 

Example is 3 divs stacked on top of each other sinc they are blocks. But we want them in the same line with margins in between.
