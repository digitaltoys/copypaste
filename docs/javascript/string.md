---
layout: default
title : String
nav_order: 2
parent : JavaScript
---

## String

```javascript
var str = "Hello world, welcome to the universe.";
var n = str.indexOf("welcome");
// 13
var n2 = str.lastIndexOf("to");
// 21
var res = str.substr(0, 5);
// hello
var res2 = str.split(" ");
// Hello,world,,welcome,to,the,universe.
var res = str.toLowerCase();
var res = str.toUpperCase();
var str = "       Hello World!        ";
str.trim();
// Hello World!

var obj = JSON.parse('{"firstName":"John", "lastName":"Doe"}');
// {firstName: "John", lastName: "Doe"}

var myObj = { "name":"John", "age":31, "city":"New York" };
var myJSON = JSON.stringify(myObj);
// "{\"name\":\"John\",\"age\":31,\"city\":\"New York\"}"
```
