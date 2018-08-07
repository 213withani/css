# Firebase App named '[DEFAULT]' already exists (app/duplicate-app)
https://github.com/zeit/next.js/issues/1999
```js
// Config file
import * as firebase from "firebase";

const config = {...};

export default !firebase.apps.length ? firebase.initializeApp(config) : firebase.app();

// Other file
import firebase from '../firebase';
...
console.log(firebase.name);
console.log(firebase.database());

```
# dont-overthink-flexbox-grids
https://css-tricks.com/dont-overthink-flexbox-grids/

# Flex
https://medium.com/@js_tut/the-complete-css-flex-box-tutorial-d17971950bdc

Parent: container
Element inside parent are items

for horizontal widths and gaps use justify
to vertically align use align

![Justify content](https://cdn-images-1.medium.com/max/800/1*V1bfijm-RCdlxcZhP7tYwA.png)
![Justify content](https://cdn-images-1.medium.com/max/800/1*XGm7JEbXLe3e9_XAdgZDYw.png)
![Justify content](https://cdn-images-1.medium.com/max/800/1*V1bfijm-RCdlxcZhP7tYwA.png)


# Flexbox — The Animated Tutorial

https://medium.com/@js_tut/flexbox-the-animated-tutorial-8075cbe4c1b2
The justify-content property determines the horizontal align of flex items. 
By default flex will not wrap your items. It works a lot like overflow: hidden;

Space between means that there is space between all inner items:

Property space-between (above) has no outer margins on corner items.
Property space-around (below) creates equal margins around all items.


# Align Content
align things vertically


# small screens
```js
/*Only do flex for screens > 900px*/
@media (min-width: 900px) {
  .careers-container {
    display: flex;
    justify-content: center;
  }
}

```
# center 3 columns 
### with same clasname
```js
.career-content {
  /* border: solid black; */
  padding: 0; /* usually part of basis and box sizing */
  margin: 10px;
  flex-basis: 30%; /* width flex way */
  box-sizing: border-box; /* easier calc */
}
```

# center 2 columns
### different width/ flex-basis

```js
.class-name-one {
  padding: 0; 
  margin: 10px;
  flex-basis: 30%; 
  box-sizing: border-box;
}

.class-name-two {
  padding: 0; 
  margin: 10px;
  flex-basis: 60%; 
  box-sizing: border-box;
}
```


# combine-flexbox-and-css-grids-for-layouts-how-to
https://getflywheel.com/layout/combine-flexbox-and-css-grids-for-layouts-how-to/

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
Example is 3 divs stacked on top of each other sinc they are blocks. But we want them in the same line with margins in between.

Container set to ```display: flex;``` will set all divs in the same line horizontally.

Flexbox strength: Equal height columns. Tricky to setup with floats.

Container/parent can set ``` align-items: flex-start ``` to use their natural height and all divs start/align at top. Size the divs based on their content, natural height and align them vertically: flex-start, flex-end, center. Default is stretch which gives us equal height.

Margins
``` margin-right: 40px``` can give you margins but last child has awkward margin.
```box-sizing: border-box; width:30%; padding: 20px``` "border-box tells the browser to account for any border and padding in the values you specify for an element's width and height." MDN

```box-sizing: border-box; flex-basis:30%; padding: 20px```
