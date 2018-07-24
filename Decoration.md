
# No decoration
## List 
https://stackoverflow.com/questions/1027354/need-an-unordered-list-without-any-bullets

```css
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
```
## Anchor tag
```css
a {
  text-decoration: none;
  color: black;
}
```

# Radio button sytling
http://selfteach.me/customizing-radio-buttons-checkboxes/
https://www.youtube.com/watch?v=hOU4Aqci2zs

```css
input[type=radio] {
  display: none;
}

input[type=radio]:checked + label {
  background:lightblue;
  border-radius: 20px;
  color: white;
}
```

http://react.tips/radio-buttons-in-reactjs/


# Nice blue color buttons
https://codepen.io/jorgebucaran/pen/zNxZLP?editors=0100

```css
body {
  align-items: center;
  background-color: #111;
  display: flex;
  font-family: Helvetica Neue, sans-serif;
  height: 100vh;
  justify-content: center;
  margin: 0;
  padding: 0;
  line-height: 1;
  text-align: center;
  color: #00caff;
}
h1 {
  color: inherit;
  font-weight: 100;
  font-size: 8em;
  margin: 0;
  padding-bottom: 15px;
}
button {
  background: #111;
  border-radius: 0px;
  border: 1px solid #00caff;
  color: inherit;
  font-size: 2em;
  font-weight: 100;
  line-height: inherit;
  margin: 0;
  outline: none;
  padding: 5px 15px 10px;
  transition: background .2s;
}
button:hover,
button:active,
button:disabled {
  background: #00caff;
  color: #111;
}
button:active {
  outline: 2px solid #00caff;
}
button:focus {
  border: 1px solid #00caff;
}
button + button {
  margin-left: 3px;
}
```
