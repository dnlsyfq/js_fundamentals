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

```
// Equal to (==) - Compares values but not types
console.log(5 == "5");  // true (different types but same value)
// Strictly equal to (===) - Compares both values and types
console.log(5 === "5");  // false (different types)
console.log(5 === 5);    // true (same type and value)
// Not equal to (!=) and strictly not equal (!==)
console.log(5 != "5");   // false (same value)
console.log(5 !== "5");  // true (different types)
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


### Initilization

```
npm init -y
npm install readline-sync

// Try to multiply text (this will cause an error)
try {
    let result = "hello" * 5;
    console.log("Result:", result);
} catch (error) {
    console.log("Oops! Something went wrong:", error.message);
}
console.log("The program continues running!");
```

```
let readline = require('readline-sync');
// Create a number for the user to guess
let secretNumber = 7;
// Get the user's guess
let userGuess = readline.question("Guess a number between 1 and 10: ");

try {
    // Convert string to number
    let numberGuess = Number(userGuess);
    
    // Check if it's actually a number
    if (isNaN(numberGuess)) {
        throw "That's not a number!";
    }
    
    // Check if number is in range
    if (numberGuess < 1 || numberGuess > 10) {
        throw "Number must be between 1 and 10!";
    }
    
    // Check if guess is correct
    if (numberGuess === secretNumber) {
        console.log("Congratulations! You guessed correctly!");
    } else {
        console.log("Sorry, the number was " + secretNumber);
    }
} catch (error) {
    console.log("Error: " + error);
}

```

```
let readline = require('readline-sync');

// Get the age
let age = readline.question("What is your age? ");

try {
    // Convert to number
    let ageNumber = Number(age);
    
    // Check if it's a valid number
    if (isNaN(ageNumber)) {
        throw "That's not a valid age!";
    }
    
    // Check if age is in valid range
    if (ageNumber < 0 || ageNumber > 120) {
        throw "Age must be between 0 and 120!";
    }
    
    // Tell them about driving
    if (ageNumber >= 16) {
        console.log("You are old enough to drive!");
    } else {
        console.log("You are not old enough to drive yet.");
    }
    
} catch (error) {
    console.log("Error: " + error);
}

```
