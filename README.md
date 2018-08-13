# Reading-Notes-JS-DOM-
Reading Notes of  "JavaScript DOM" "DOM Scripting- Web Design with JavaScript and the Document Object Model"

##### In the next few days, I will update the other chapters and exercises of the examples.

## Chapter 7
### Creating Markup on The Fly
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







