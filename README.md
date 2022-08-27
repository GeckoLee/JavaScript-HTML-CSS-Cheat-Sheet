# JavaScript HTML CSS Cheat Sheet
 My personal Cheat Sheet with commonly used expressions

# Div Selector

```javascript
const div_by_id = document.getElementById('idname');
const div_by_class = document.querySelector('.classname');
```

# Timeout

```javascript
setTimeout(function(){

}, 1000);
```

<hr>

```javascript
myTimeout = setTimeout(function(){

}, 100);
```

```javascript
clearTimeout(myTimeout);
```

# CSS orientation

```
@media (orientation: landscape) {}

@media (orientation: portrait) {}
```

# Random Number between a & b

```javascript
let rnd=(a,b)=>~~(Math.random()*(b-a))+a;
```

<hr>

String to Integer
```javascript
parseInt(a);
```

<hr>

Pad Integer i into string of size 2 with leading 0
```javascript
String(i).padStart(2, '0');
```

# Object - Output object content with unknown property names

```javascript
let object_property_array = Object.getOwnPropertyNames(obj);
for(let i=0;i<object_property_array.length;i++){
  console.log(obj[object_property_array[i]]);
}
```

# Modify CSS Style Sheet
```javascript
function Modify_StyleSheet(){
  const stylesheet = document.styleSheets[0];
  let bodyRules;
  let elementRules;
  let selector = '.classname';

  for(let i = 0; i < stylesheet.cssRules.length; i++) {
    if(stylesheet.cssRules[i].selectorText === 'body') {
      bodyRules = stylesheet.cssRules[i];
    }
    if(stylesheet.cssRules[i].selectorText === selector) {
      elementRules = stylesheet.cssRules[i];
    }
  }

  console.log(bodyRules);
  bodyRules.style.setProperty('padding', '4vw');
  // modifying the rule in the stylesheet
  elementRules.style.setProperty('width', setting_field_size_width+'px');
}
```
