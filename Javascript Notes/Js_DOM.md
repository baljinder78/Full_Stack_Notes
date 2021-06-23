# Javascript DOM

## what is DOM ?

**DOM** stands for **Document Object Model**

Javascript DOM is known as **HTML DOM**

## what does HTML DOM mean?

The HTML DOM is a standard for how to get, change, add, or delete HTML elements

The HTML DOM is a standard object model and programming interface for HTML. It defines:

- The HTML elements as **objects**
- The **properties** of all HTML elements
- The **methods** to access all HTML elements
- The **events** for all HTML elements


## Methods
HTML DOM methods are **actions** you can perform.

## Properties
HTML DOM properties are **values** that you can set or change.

## objects
In the DOM, all HTML elements are defined as **objects**.

## Events
HTML DOM events are the **functionalites** you can preforme. 


lets understand with example 

for example:-

``` html
<!DOCTYPE html>
<html>
<body>

<h2 id="demo">My First Page</h2>

<button onclick="fun()">clcik me</button>

<script>
    function fun()
    {
        document.getElementById("demo").innerHTML ="Hello World!";
    }

</script>

</body>
</html>
```

here in given example :-

**objects** are ***html, body, h2, p, script***.

**Method** is ***getElementById***.

**Propertie** is ***innerHTML***.

**event** is ***onclick***.