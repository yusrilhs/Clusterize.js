# Clusterize.js
> This is fork version from clusterize.js. I just add filter callback and modify update method

[Demo, usage, etc…](https://clusterize.js.org/)

## Example filter
```js
var clusterize = new Clusterize({
  scrollId: 'scrollArea',
  contentId: 'list-group',
  tag: 'a',
  filter: function(row) {
    // Row is text without html tag
    return row.toUpperCase().indexOf(search.value.toUpperCase()) > -1
  }
})

// Call update the update without new rows parameter
clusterize.update()
```
