# Search
https://www.youtube.com/watch?v=wXDFOgkR4kk

https://stackoverflow.com/questions/1457849/how-to-remove-the-border-highlight-on-an-input-text-element

```css
export const Search = styled.input` 
  width: 200px;
  padding: 7px; 
  border: 1px solid ${_grey};
  &:focus {
    outline-width: 0;
  }
`

export const Submit = styled.input` 
  background: ${_grey};
  padding: 7px; 
  border: 1px solid ${_grey};
  margin-left: -5px;
  cursor: pointer;
  color: white;
  
  &:hover{
    background: #333;
    transition: all .40s;
  }
`
```
