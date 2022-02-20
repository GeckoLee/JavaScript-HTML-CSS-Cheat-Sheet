# JavaScript HTML CSS Cheat Sheet
 My personal Cheat Sheet with commonly used expressions

# Div

const div_grid = document.getElementById('');

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

@media (orientation: landscape) {
}
@media (orientation: portrait) {
}

# Random Number between a & b

let rnd=(a,b)=>~~(Math.random()*(b-a))+a;
