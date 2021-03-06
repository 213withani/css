# rem - relative unit
5rem is 5 times the core element size.

# view port (vh/vw)
https://css-tricks.com/fun-viewport-units/
The difference between % and vw is most similar to the difference between em and rem. A % length is relative to local context (containing element) width, while a vw length is relative to the full width of the browser window.

# pseudo firstChild
```
listItem: {
    display: 'flex',
    alignItems: 'center',
    justifyContent: 'center',
    height: `${MENU_ITEM}px`,
    cursor: 'pointer',
    ':firstChild': {
      paddingLeft: '0',
    },
    border: 'solid green'
  },
```

# ReactJS Calendar

https://www.youtube.com/watch?v=9U0uTNfY1UA

# Learn CSS in 12 Minutes
https://youtu.be/0afZj1G0BIE

## Layout
* Everything is a div, create a #container and then #rows inside and inside those rows create #columns if necessary. Simple layout with rows and columns.
* In html it is good to define rows and then split the rows up into columns if necessray. 

## 800 px
https://www.quora.com/How-much-is-800-pixels
We think of pixels as a more relative unit because their size will be different on different devices. a high resolution device will have more pixels per inch/cm and thus the pixels will be smaller.


* commas are used to shared properties between elements.
* spaces are used to be more specific. You can drill down inside nested elements, thus a long chain separated by spaces can be createda.

## Relationship / link
<link rel type href />

## center container div
```
# container {
   margin-left auto;
   margin-right auto;
}
```

## floating
``` clear:both ``` Lets get past all the floating elements and then display.

## separated is being more specific
* ids and classes space separated is being more specific
* But ul has to be nested inside nav
```
#nav ul{
 list-style-type: none;
}
```

# a link text decoration is none

# font
``` font-family: Heveltica, Arial, sans-serif; ```

## separated by comma 
Means sharing 

```
#header, .sidebar {
 color: blue;
}
```

# style in header

Add css directly in html
```
<head>
 #header {
  color: blue;
 }
</head>
```

## Inline
