# Js DOM Finding HTML Elements

>**In javascript we usually work manipulate HTML elements.**

for doing this we first need to find element.
In dom we have some methods to find element/elements.

*Those methods are*:
- Finding HTML element by ***id***
- Finding HTML elements by ***tag name***
- Finding HTML elements by ***class name***
- Finding HTML elements by ***CSS selectors***
- Finding HTML elements by ***HTML object collections***


## 1. Finding HTML Element by Id
id is unique key given to Html tag.

finding element by id always return single element.

example of id:-
```HTML
<p id="intro">here "intro" is id</p>
```
in given example *"intro"* is a id.

to find elemement by id in js dom the syntax is
```js
document.getElementById("demo")
```
here *"demo"* is the id 

eg:-
```jsx
<!DOCTYPE html>
<html>
<body>


<p id="intro">Finding HTML Elements by Id</p>

<button onclick="byid()">try me</button>

<script>
function byid()
{
	document.getElementById("intro").innerHTML="The text is changed when clicked on button";
}
</script>

</body>
</html>
```

here when you click on button innercontent of tag with id *"intro"* changed.

## 2.Finding HTML Elements by Tag Name
every element is know as tag in HTML.

Finding elements by tag name returns list of elements having the given tag

example:-
```HTML
<h2>Heading tag</h2>
<p>paragraph tag</p>
<div>div tag</div>
```
here tags are *" [ h2, p, div ] "*.

to find elements by tagname in js dom the syntax is
```js
document.getElementsByTagName("p")
```
here you will get list of paragraph( *"p"* ) tag.

example:-
```html
<!DOCTYPE html>
<html>
<body>


<p>paragraph 1</p>
<p>paragraph 2</p>
<button onclick="byid()">try me</button>

<script>
function byid()
{
	document.getElementsByTagName("p")[0].innerHTML="The text in paragraph 1 changed  is changed when clicked on button";
}
</script>

</body>
```

when button is clicked the inntertext of first paragraph tag will be changed.


## 3.Finding HTML Elements by Class Name
class in html is used to represent group of tags.

Finding elements by class name returns list of elements having the given class name

example:-
```HTML
<h2 class="demo">Heading tag</h2>
<p class="demo">paragraph tag</p>
<div>div tag</div>
```
here the elements with class *"demo"* are *" [ h2, p ] "*.

to find elements by class name in js dom the syntax is
```js
document.getElementsByClassName("demo")
```
here you will get list of tags having class  *"demo"*.

example:-
```html
<!DOCTYPE html>
<html>
<body>
<h2> heading without class</h2>
<h2 class="demo">Heading with class</h2>
<p class="demo">paragraph tag</p>
<div>div tag</div>
<button onclick="byid()">try me</button>

<script>
function byid()
{
	document.getElementsByClassName("demo")[0].innerHTML="The text in h2 tag with class demo is changed when clicked on button";
}
</script>

</body>
```

when button is clicked the inntertext of the h2 tag with class *"demo"* will be changed.

## 4.Finding HTML Elements by CSS Selectors
In Html CSS selectors  are ***(id, class names, types, attributes, values of attributes, etc)***

Finding elements by CSS Selector returns list or a single element having the given CSS Selector

example:-
```HTML
<h2> heading without class</h2>
<h2 class="demo">Heading1 with class</h2>
<h2 class="demo">Heading2 with class</h2>
<p class="demo">paragraph tag</p>
<div id="one">div tag</div>
```
here the elements with css selector *".demo"* are *" [ second h2, p ] "*.

to find elements by Css selector in js dom the syntax is
```js
document.querySelectorAll("h2.demo"); //list of h2 tag with class demo

document.querySelector("div#one"); //a div tag with id one
```

example:-
```html
<!DOCTYPE html>
<html>
<body>
<h2> heading without class</h2>
<h2 class="demo">Heading with class</h2>
<p class="demo">paragraph tag</p>
<div id="one">div tag</div>
<button onclick="byid()">try me</button>
<button onclick="byid2()">try me2</button>

<script>
function byid()
{
	document.querySelectorAll("h2.demo")[0].innerHTML="The text in h2 tag with class demo is changed when clicked on button";
}
function byid2()
{
	document.querySelector("div#one").innerHTML="The text in div with id one is changed when clicked on button";
}
</script>

</body>
```

when button "tryme" is clicked the inntertext of the h2 tag with class *"demo"* will be changed.

when button "tryme2" is clicked the inntertext of the div tag with id *"one"* will be changed.

