# <p align="center">JavaScript Bootcamp Assignments</p>

Current Progress : <p>![](https://progress-bar.dev/18/?scale=100&width=1100)</p>

### Week 1: Introduction - from 1 to 9

###### Assignment 1
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <title>Learn JavaScript</title>
    <script>
      // this will cause an error. the element "el" hasn't load in the document yet
      document.getElementById("el").style.color = "red";
    </script>
    <script>
      // this won't cause an error. the code will be called when the window load so it's okay 
      window.onload = function () {
        document.getElementById("el").style.color = "red";
      };
    </script>
  </head>
  <body>
    <h1 id="el">Page Title</h1>
    <script>
      // this won't cause an error. the element "el" loaded already
      document.getElementById("el").style.color = "red";
    </script>
  </body>
</html>
```
###### Assignment 2
```
document.write(`<h1 style="color: blue;
font-size: 80px;
font-weight: bold;
text-align: center;
font-family: Arial">ELZERO</h1>`);
```
###### Assignment 3
```
console.log("%cElzero %cWeb %cSchool", "color:red; font-size:40px", "color:green; font-size:40px; font-weight:bold", "color:white; font-size:40px; background-color:blue")
```
###### Assignment 4
```
console.group("Group 1");
console.log("Message One");
console.log("Message Two");
console.group("Child Group");
console.log("Message One");
console.log("Message Two");
console.group("Grand Child Group");
console.log("Message One");
console.log("Message Two");
console.groupEnd();
console.groupEnd();
console.groupEnd();
console.group("Group 2");
console.log("Message One");
console.log("Message Two");
console.groupEnd();
```
###### Assignment 5
```
console.table(["ash","roaa","Mohammed","Hamdy"])
```
###### Assignment 6
```
// First method
// console.log("Iam In Console");
// document.write("Iam In Page");

/* Second method */
/*
console.log("Iam In Console");
document.write("Iam In Page");
*/
```

### Week 2: Data Types And Variables - from 10 to 17

###### Assignment 1
```
var number1 = 10;
var number2 = 20;

console.log(number1+""+number2); 
console.log(typeof (number1+""+number2)); 
console.log(`${number1}${number2}`); 
console.log(typeof(`${number1}${number2}`)); 

console.log(number2+"\n"+number1);

console.log(`${number1}
${number2}`);
```
###### Assignment 2
```
<div id="elzero">object</div>
```
###### Assignment 3
```
console.log("I'm In \n\\\\\nLove \\\\\"\"\" '''\n++ With ++ \n\\\"\"\"\\\"\"\"\n\"\"JavaScript\"\"`")
```
###### Assignment 4
```
console.log("_" + `${a}_${b}`.repeat(4) + "_");
```

### Week 3: Operators - from 18 to 22

###### Assignment 1
```
console.log(10 * 20 + (15 % 3) + 190 + 10 - 400)
```
###### Assignment 2
```
let num = 3;

// Solution One
console.log(num + true + true + true); // 6

// Solution Two
console.log(num * (true + true)); // 6

// Soultion Three
console.log(num - (false - (true + true + true))); // 6

// Soultion Four
console.log((true + true) * (true + true + true)); // 6

// Solution Five
console.log(true + true + true + true + true + true); // 6

// Solution Six
console.log(++num + (true + true)); // 6
```
###### Assignment 3
```
let num = "10";

// Solution One
console.log(+num * (true + true)); // 20

// Solution Two
console.log(+num + +num); // 20

// Solution Three
console.log(num++ + --num); // 20

// Solution Four
console.log(Number(num) + +num); // 20
```

### Week 4: Numbers And Strings - from 23 to 30 

###### Assignment 1.1
```
console.log(100_000);
console.log(100000);
console.log(5e4 + 5e4);

console.log(10 * 10 * 10 * 10 * 10);
console.log(10 ** 5);
console.log(Math.pow(10, 5));
console.log(Math.ceil(99999.9));
console.log(Math.floor(100000.1));
console.log(Math.round(100000.1));
console.log(Math.trunc(100000.5));
console.log(Number("100000"));
console.log(+"100000");
console.log(parseInt("100000"));
```
###### Assignment 1.2
```
console.log(-Number.MIN_SAFE_INTEGER)
```
###### Assignment 1.3
```
console.log(Number.MAX_SAFE_INTEGER.toString().length)
```
###### Assignment 1.4
```
let myVar = "100.56789 Views";

console.log(parseInt(myVar));
console.log(+parseFloat(myVar).toFixed(2)); 
```
###### Assignment 1.5
```
let num = 10;

console.log(Number.isInteger(num) + Number.isInteger(num));
```
###### Assignment 1.6
```
let flt = 10.4;

console.log(Math.trunc(flt));
console.log(Math.floor(flt));
console.log(Math.round(flt));
console.log(parseInt(flt));
console.log(Number(flt.toFixed(0)));
```
###### Assignment 1.7
```
console.log(Math.floor(Math.random()*5) ); 
```

### Control Flow
> To be added


### Arrays
> To be added


### Loop
> To be added


### Functions & Scope
> To be added


### Higher Order Functions And Practice
> To be added


### Objects
> To be added

