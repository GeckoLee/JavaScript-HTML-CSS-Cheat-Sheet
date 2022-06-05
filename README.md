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

# Object - Output object contents with unknown property names

```javascript
let object_property_array = Object.getOwnPropertyNames(obj);
for(let i=0;i<object_property_array.length;i++){
  console.log(obj[object_property_array[i]]);
}
```
