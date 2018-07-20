
# No decoration
## List 
https://stackoverflow.com/questions/1027354/need-an-unordered-list-without-any-bullets

```js
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
```
## Anchor tag
```js
a {
  text-decoration: none;
  color: black;
}
```

# Radio button sytling
http://selfteach.me/customizing-radio-buttons-checkboxes/
https://www.youtube.com/watch?v=hOU4Aqci2zs

```js
input[type=radio] {
  display: none;
}

input[type=radio]:checked + label {
  background:lightblue;
  border-radius: 20px;
  color: white;
}
``

http://react.tips/radio-buttons-in-reactjs/
