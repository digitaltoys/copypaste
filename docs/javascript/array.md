---
layout: default
title : Array
nav_order: 1
parent : JavaScript
---

# Array

```javascript
var a = [21, 16];
var b = [54, 4, 2];
var c = a.concat(b); 
// 21,16,54,4,2

c.filter((item) => item>10);
// 21,16,54
c.find((item) => item>30);
// 54
c.forEach((item, index)=> c[index]=item+10);
// c=[31,26,64,14,12]
c.indexOf(4);
// 3
c.join(":");
// 31:26:64:14:12
c.keys();
// 0,1,2,3,4
c.pop();
// c=[31,26,64,14]
c.push(22);
// c=[31,26,64,14,22]
c.shift()
// c=[26,64,14,22]
c.unshift(19,3)
// c=[19,3,26,64,14,22]
c = c.slice(1, 5);
// c=[3,26,64,14]
c = c.map((item)=>i+1);
// c=[20, 4, 27, 65, 15, 23]
c.reduce((sum,i)=> sum+i);
// 148
```
