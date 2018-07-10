
# CSS Grid
https://www.youtube.com/watch?v=jV8B24rSN5o

Flexbox: 1 dimensional layout for columns or rows.

Grid: 2D Dimensional layouts for columns and rows.

2 divs, 2 columns, if you add more it will add it and keep two columns.
```
display:grid;
grid-template-columns: 70% 30%; // creates two columns
```

3 columns:
```
grid-template-columns: 40% 30% 30%; // creates two columns
```

Margin with same spacing for column and row:
```
grid-gap: 1em;
```

```
display:grid;
grid-template-columns: 1fr 2fr 1fr; // creates 3 columns with one being twice the size of the others.
```

```
1fr 1fr 1fr 1fr  same as repeat(4, 1fr)
```

fixed heights, 100px with content doesn't matter. This is not content flexible.
```
grid-auto-rows: 100px;
```

100px by default but will stretch out to fill the content if content is > 100px. Only the row with bigger content will stretch, other rows stay at their min height.

```
grid-auto-rows: minmax(100px,auto);
```

## You can nest grids.
## Justifying and aligning items

column will fit content

justify-items default is stretch.

justify-items will align start of column, left and column will fit content horizontally.
```
display:grid;
grid-template-columns: 1fr 2fr 1fr;
grid-auto-rows: minmax(100px, auto);
grid-gap: 1em;
justify-items: start;
```

default is stretch, you can use ```start, center, end```

```align-items:``` column will fit content verically.

```
align-items: start; // start of top, align top vertically
align-items: center; // midway
align-items: start; // bottom
align-items: stretch; // default, fills column
```

All items at once  using ```justify-items``` or individually using ```justify-self ```.

All items at once using ```align-items``` or individually using ```align-self ```.

```
align-self:start;
align-self:start;
align-self:start;
align-self:start;
```

## Grid Columns using line numbers

From column line 1 to 3

```
grid-column:1/3
```

From row line 1 to 3

```
grid-row:1/3
```

Columns and rows can overlap. This is not possible with flexbox.

```
```
