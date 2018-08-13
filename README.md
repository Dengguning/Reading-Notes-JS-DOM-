# Reading-Notes-JS-DOM-
Reading Notes of  "JavaScript DOM" "DOM Scripting- Web Design with JavaScript and the Document Object Model"

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

```javascript
function insertParagraph(text) {
var str = "<p>";
str += text;
str += "</p>";
document.write(str);
}
```


