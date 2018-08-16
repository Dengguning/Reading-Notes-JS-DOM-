# Reading-Notes-JS-DOM-
Reading Notes of  "JavaScript DOM" "DOM Scripting- Web Design with JavaScript and the Document Object Model"

##### In the next few days, I will update the other chapters and exercises of the examples.

## Chapter 3

## Chapter 4

## Chapter 5

## Chapter 6

## Chapter 7
### Creating Markup on The Fly
[Show the gallery]()
#### What this chapter covers:
* "old school" techniques: document.write and innerHTML
* DOM methods createElement, createTextNode, appendChild and insertBefore

##### document.write
```javascript
<script>
  document.write("<p>This is inserted.</p>");
</script>
```

An external file: xxx.js
```javascript
function insertParagraph(text) {
  var str = "<p>";
  str += text;
  str += "</p>";
  document.write(str);
}
```

Before /body
```javascript
<script>
  insertParagraph("This is inserted.")
</script>
```

##### InnerHTML
```html
<div id="testdiv">
</div>
```

An external file: xxx.js
```javascript
window.onload = function() {
  var testdiv = document.getElementById("testdiv");
  testdiv.innerHTML = "I inserted this content.";
}
```


####  DOM methods

##### createElement

This is a two-step process.
1.Create the new element.
2.Insert the element into the node tree.

This is the syntax:
```javascript
document.createElement(nodeName);
```

This statement will create a paragraph element:
```javascript
document.createElement("p");
```

It's a gooed idea to assign the newly created element to a variable:
```javascript
var para = document.createElement("p");
```

An external file: xxx.js:

```javascript
window.onload = funcion {
  var para = document.createElement("p"); 
  var info = "nodeName"; 
  info += para.nodeName; 
  info += " nodeType: "; 
  info += para.nodeTYpe; 
  alert(info); 
}
```












