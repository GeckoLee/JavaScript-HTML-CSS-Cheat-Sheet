# JavaScript HTML CSS Cheat Sheet
 My personal Cheat Sheet with commonly used expressions

# Div Selector

const div_by_id = document.getElementById('idname');
const div_by_class = document.querySelector('.classname');

<hr>

# Timeout

setTimeout(function(){

}, 1000);

<hr>

myTimeout = setTimeout(function(){

}, 100);

clearTimeout(myTimeout);

<hr>

# CSS orientation

@media (orientation: landscape) {}

@media (orientation: portrait) {}

<hr>

# Random Number between a & b

let rnd=(a,b)=>~~(Math.random()*(b-a))+a;

<hr>

String to Integer
parseInt(a);

<hr>

Pad Integer i into string of size 2 with leading 0
String(i).padStart(2, '0')

<hr>

# Object - Output object contents with unknown property names

let object_property_array = Object.getOwnPropertyNames(current_album[id]);
for(let i=0;i<object_property_array.length;i++){
  console.log(current_album[id][object_property_array[i]]);      
}
