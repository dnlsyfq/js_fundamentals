**data types**
* string
* number
* boolean
* null // absence of value
* undefined // not yet assigned a value
* bigint // greater range of number
* symbol // unique identifier 

* Operator
```
let timeRemaining = 0
let energy = 10

console.log(`Game over: ${timeRemaining == 0 || energy == 0}`)
```

* boolean
```
true
false
```

* typeof
```
typeof var
```

* convert string to integer
```
parseInt(var)
```
* unary operator
```
+ prompt(' ')
```

* convert string to float
```
parseFloat(var)
```

* String Interpolation
```
console.log(`Hello ${firstName} ${lastName}`)
```

* Arrow Function Syntax
```
const lineBreak = () => console.log("");
```

* Debugging



* object
```
var king = { firstName: "Ned", lastName:"Stark", age:40};

Object.keys(king);

["firstName", "lastName", "age"]
```

* if

```
if(condition){
}
```

* for
```
for(initiation; condition; update){
}
```

* array
```
array.length
array.push(var) // add element to the last
```

* math
```
const secsPerMin = 60;
const minsPerHour = 60;
const hoursPerDay = 24;
const daysPerWeek = 7;
const weeksPerYear = 52;

const secondsPerDay = hoursPerDay * minsPerHour * secsPerMin;

let sentence = document.querySelector('main')
sentence.innerHTML = `<h1>There are ${secondsPerDay} seconds in a day.</h1>`;

const yearsAlive = 34 * weeksPerYear * daysPerWeek * hoursPerDay * minsPerHour * secsPerMin;
sentence.innerHTML += `<h2>I've been alive for more than ${yearsAlive} seconds!</h2>`;
```
