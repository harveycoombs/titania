# Titania is a lightweight, yet powerful JavaScript library.

## Frequently Asked Questions
### What can Titania do?
Titania provides an environment for developing concise & effective JavaScript. Besides simplifying DOM manipulation, Titania also provides tools for parsing, calculations & HTTP requests.

### Why should I use Titania over other libraries?
Titania includes various useful tools & routines for convenience. Other libraries do not include said features & are often provably slower than Titania.
Additionally, Titania aims to limit the deprecation of features to ensure the stability of those who include the latest version in their projects.

### I'm sold! How do I use/learn Titania?
You can download Titania, at any time, from [this repository](https://github.com/harveycoombs/titania/).
Alternatively, you can include the following script tag in your project:<br/>
`<script src="http://harveycoombs.com/titania/releases/latest/titania.js" type="text/javascript" crossorigin="anonymous"></script>`

## Examples

### Adding classes to DOM elements
```js
//Native JavaScript
var box = document.querySelector("#box");
box.classList.add("classX", "classY", "classZ");

//Titania JavaScript
var box = DOM.select("#box");
box.apply("classX classY classZ");
```

### Attaching & detaching Event listeners
```js
//Native JavaScript
var item = document.querySelector("div.item");

item.addEventListener("click", function () {
  console.log("I was clicked!");
});

//Titania JavaScript
var item = DOM.select("div.item");

item.listen("click", function () {
  console.log("I was clicked!");
});
```

More tips, tricks & examples can be found within Titania's [Documentation](http://harveycoombs.com/titania/docs).
