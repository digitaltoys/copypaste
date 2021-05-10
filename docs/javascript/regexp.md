---
layout: default
title : RegExp
parent : JavaScript
has_children: false
nav_order: 3
---

## RegExp

### Character classes
.	any character except newline  
\w\d\s	word, digit, whitespace  
\W\D\S	not word, digit, whitespace  
[abc]	any of a, b, or c   
[^abc]	not a, b, or c  
[a-g]	character between a & g  
a* a+ a?	0 or more, 1 or more, 0 or 1  

### Anchors
^abc$	start / end of the string  
\b\B	word, not-word boundary  
### Escaped characters
\.\*\\	escaped special characters  
\t\n\r	tab, linefeed, carriage return  

### group
(ABC)    capture group  
(?<name>ABC) named capture group  
\1       numeric reference  
(?:ABC)  non capture group  
  
### Lookaround
(?=ABC) positive lookahead  
(?!ABC) negative lookahead  
(?<=ABC) positive lookbehind  
(?<!ABC) negative lookbehind  

```javascript
a="1pt 2px 3em 4px"
a.match(/\d(px)/g)
// ["2px", "4px"]

a.match(/\d(?=px)/g)
// ["2", "4"]

a.match(/\d(?!px)/g)
// ["1", "3"]
```
