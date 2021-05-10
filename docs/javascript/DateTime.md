---
layout: default
title : DateTime
parent : JavaScript
has_children: false
nav_order: 3
---

# DateTime

### using
https://momentjs.com/docs/#/use-it/  
```javascript
// node.js
import moment from "moment";
// browser
<script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.1/moment.min.js" integrity="sha512-qTXRIMyZIFb8iQcfjXWCO8+M5Tbc38Qi5WzdPOYZHIlZpzBHG3L3by84BBBOiRGiEb7KKtAOAs5qYdUiZiQNNQ==" crossorigin="anonymous"></script>
```

### Format Dates
```javascript
moment().format('MMMM Do YYYY, h:mm:ss a'); // May 10th 2021, 2:32:17 pm
moment().format('dddd');                    // Monday
moment().format("MMM Do YY");               // May 10th 21
moment().format('YYYY [escaped] YYYY');     // 2021 escaped 2021
moment().format();                          // 2021-05-10T14:32:17+09:00
```
### Relative Time
```javascript
moment("20111031", "YYYYMMDD").fromNow(); // 10 years ago
moment("20120620", "YYYYMMDD").fromNow(); // 9 years ago
moment().startOf('day').fromNow();        // 15 hours ago
moment().endOf('day').fromNow();          // in 9 hours
moment().startOf('hour').fromNow();       // 32 minutes ago
```
### Calendar Time
```javascript
moment().subtract(10, 'days').calendar(); // 04/30/2021
moment().subtract(6, 'days').calendar();  // Last Tuesday at 2:32 PM
moment().subtract(3, 'days').calendar();  // Last Friday at 2:32 PM
moment().subtract(1, 'days').calendar();  // Yesterday at 2:32 PM
moment().calendar();                      // Today at 2:32 PM
moment().add(1, 'days').calendar();       // Tomorrow at 2:32 PM
moment().add(3, 'days').calendar();       // Thursday at 2:32 PM
moment().add(10, 'days').calendar();      // 05/20/2021
```
