# <p align="center">JavaScript Bootcamp Assignments</p>

Current Progress : <p>![](https://progress-bar.dev/50/?scale=100&width=1100)</p>
<hr>

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
<hr>

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
<hr>

### Week 3: Operators - from 18 to 22

###### Assignment 1
```
console.log(10 * 20 + (15 % 3) + 190 + 10 - 400)
```
###### Assignment 2
```
let num = 3;

// Solution One
console.log(num + true + true + true); 

// Solution Two
console.log(num * (true + true)); 

// Soultion Three
console.log(num - (false - (true + true + true)));

// Soultion Four
console.log((true + true) * (true + true + true)); 

// Solution Five
console.log(true + true + true + true + true + true); 

// Solution Six
console.log(++num + (true + true)); 
```
###### Assignment 3
```
let num = "10";

// Solution One
console.log(+num * (true + true)); 

// Solution Two
console.log(+num + +num); 

// Solution Three
console.log(num++ + --num); 

// Solution Four
console.log(Number(num) + +num); 
```
<hr>

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
<br>

###### Assignment 2.1
```
let userName = "Elzero";
console.log(userName[0].toLowerCase());
console.log(userName.charAt(0).toLowerCase());
console.log(userName.substring(0, 1).toLowerCase());
console.log(userName.slice(0, 1).toLowerCase());
console.log(userName.substr(0, 1).toLowerCase());
console.log(userName.split("", 1).toString().toLowerCase().repeat(3)); 
```
###### Assignment 2.1
```
let word = "Elzero";
let letterZ = "z";
let letterE = "e";
let letterO = "O";

console.log(word.includes(letterZ)); 
console.log(word.startsWith(letterE.toUpperCase())); 
console.log(word.endsWith(letterO.toLowerCase())); 
```
<hr>

### Week 5: Control Flow - from 31 to 39  

###### Assignment 1.1
```
console.log(100 == "100");
console.log(100 < 1000);
console.log(110 > 100 || 10 < 20);
console.log(-10 == "-10");
console.log(!-50 >= +"-40");
console.log(!10 <= -"-40");
console.log(!"10" != 10);
console.log(!20 == false);
```
###### Assignment 1.2
```
let num1 = 10;
let num2 = 20;

console.log(typeof num1 === typeof num2); 
console.log(num1 < num2); 
console.log(num2 > num1); 
console.log(!(num1 == num2)); 
console.log(num1 != num2); 
console.log(num1 <= num2); 
```
###### Assignment 1.3
```
let a = 20;
let b = 30;
let c = 10;

console.log(a < b && a > c || a == b); 
console.log(a < b || a != c); 
console.log(!(a == b) && !(a > b) && !(a == c) && !(a < c));
```
<br>

###### Assignment 2.1
```
// Test Case 1
// let num = 9; // "009"

// Test Case 2
// let num = 20; // "020"

// Test Case 3
// let num = 110; // "110"

if (num.toString().length == 1) {
  console.log(`00${num}`);
} else if (num.toString().length == 2) {
  console.log(`0${num}`);
} else {
  console.log(num);
}
```
###### Assignment 2.2
```
let num1 = 9;
let str = "9";
let str2 = "20";

if (num1 == str) {
  console.log(`{num1} Is The Same Value As {str}`);
} else if (num1 == str && num1 !== str) {
  console.log(`{num1} Is The Same Value As {str} But Not The Same Type`);
} else if (num1 !== str2) {
  console.log(`{num1} Is Not The Same Value Or The Same Type As {str2}`);
} else if(typeof str === typeof str2 && str != str2){
    console.log(`{str} Is The Same Type As {str2} But Not The Same Value`)
}
```
###### Assignment 2.3
```
let num1 = 10;
let num2 = 30;
let num3 = "30";

num3 > num1 && num3 !== num2
  ? console.log(
      "30 Is Larger Than 10 And Type string Not The Same Type As number"
    )
  : num3 > num1 && num3 == num2 && typeof num3 !== typeof num2
  ? console.log(
      "30 Is Larger Than 10 And Value Is The Same As 30 And Type string Not The Same Type As number"
    )
  : num3 !== num1 && typeof num3 !== typeof num2
  ? console.log(
      "{num3} Value And Type Is Not The Same As {num1} And Type Is Not The Same As {num2}"
    )
  : "";
```
###### Assignment 2.4
```
// Edit What You Want Here

let num1 = 15;
let num2 = 6;
let num3 = 15;
let num4 = 45;
num4 - (num1 + num3) + num2 === 21;

// Condition 1

if (num1 > num2) {
  console.log("True");
} else {
  console.log("False");
}

// Condition 2

if (num1 > num2 && num1 < num4) {
  console.log("True");
} else {
  console.log("False");
}

// Condition 3

if (num1 > num2 && num1 === num3) {
  console.log("True");
} else {
  console.log("False");
}

// Condition 4

if (num1 + num2 < num4) {
  console.log("True");
} else {
  console.log("False");
}

// Condition 5

if (num1 + num3 < num4) {
  console.log("True");
} else {
  console.log("False");
}

// Condition 6

if (num1 + num2 + num3 < num4) {
  console.log("True");
} else {
  console.log("False");
}

// Condition 7

if (num4 - (num1 + num3) + num2 === 21) {
  console.log("True");
} else {
  console.log("False");
}
```
<br>

###### Assignment 3.1
```
let day = "   tuesday  ";
day = day.trim();
day = day.charAt(0).toUpperCase() + day.slice(1);

switch (day) {
  case "Friday":
  case "Saturday":
  case "Sunday":
    console.log("No Appointments Available");
    break;
  case "Monday":
  case "Thursday":
    console.log("From 10:00 AM To 5:00 PM");
    break;
  case "Tuesday":
    console.log("From 10:00 AM To 6:00 PM");
    break;
  case "Wednesday":
    console.log("From 10:00 AM To 7:00 PM");
    break;
  default:
    console.log("Its Not A Valid Day");
}
```
<hr>

### Week 5: Arrays - from 40 to 47  

###### Assignment 1
```
let myFriends = ["Ahmed", "Elham", "Osama", "Gamal"];
let num = 3;

// Method 1
console.log(myFriends.slice(0, num)); // ["Ahmed", "Elham", "Osama"];

// Method 2
myFriends.length = num;
console.log(myFriends); // ["Ahmed", "Elham", "Osama"];
```

###### Assignment 2
```
let friends = ["Ahmed", "Eman", "Osama", "Gamal"];
friends.shift();
friends.pop();
console.log(friends); // ["Eman", "Osama"]
```

###### Assignment 3
```
let arrOne = ["C", "D", "X"];
let arrTwo = ["A", "B", "Z"];
let finalArr = [];

finalArr = finalArr.concat(arrOne, arrTwo).sort().reverse();
console.log(finalArr); // ["Z", "X", "D", "C", "B", "A"]
```

###### Assignment 4
```
let website = "Go";
let words = [`${website}ogle`, "Facebook", ["Elzero", "Web", "School"]];

console.log(words[words.length - true][0].toUpperCase().slice(website.length)); 
```
###### Assignment 5
```
let needle = "JS";
let haystack = ["PHP", "JS", "Python"];

if (haystack.includes(needle)) {
  console.log(`Found`);
}
if (haystack.indexOf("needle" != -1)) {
  console.log(`Found`);
}
if (haystack.lastIndexOf("needle" != -1)) {
  console.log(`Found`);
}
```

###### Assignment 6
```
let arr1 = ["A", "C", "X"];
let arr2 = ["D", "E", "F", "Y"];
let allArrs = [];

// Your Code Here
allArrs = allArrs
  .concat(arr1, arr2)
  .sort()
  .slice(arr2.length)
  .join("")
  .toLowerCase();

console.log(allArrs); // fxy
```
<hr>

### Week 6: Loops - from 48 to 56

###### Assignment 1.1
```
let start = 10;
let end = 100;
let exclude = 40;

for (let i = start; i <= end; i += start) {
  if (i == exclude) {
    continue;
  }
  console.log(i);
}
```
###### Assignment 1.2
```
let start = 10;
let end = 0;
let stop = 3;

for(let i = start; i>=stop; i--){
    if(i>=start){
        console.log(i.toString())
    }
    else{
        console.log(`${end}${i}`)
    }
}
```
###### Assignment 1.3
```
let start = 1;
let end = 6;
let breaker = 2;

for (let i = start; i <= end; i++) {
  console.log(i);
  for (let k = breaker; k < breaker ; k += breaker) {
    console.log(`-- ${k}`);
  }
}
```
###### Assignment 1.4
```
let index = 10;
let jump = 2;
let end = 0;

for (;;) {
    console.log(index);
    if (index === jump * jump) break;
    index -= jump;
}
```
###### Assignment 1.5
```
let friends = ["Ahmed", "Sayed", "Eman", "Mahmoud", "Ameer", "Osama", "Sameh"];
let letter = "a";
let ctn = +false;

for (let i = +false; i < friends.length;i++) {
  if (friends[i].startsWith(letter.toUpperCase())) continue;
  console.log(`${++ctn} => ${friends[i]}`);
}
```
###### Assignment 1.6
```
let start = 0;
let swappedName = "elZerO"; // ELZERO
let final = "";

let upperName = swappedName.toUpperCase();

for (let i = start; i < swappedName.length; i++) {
  if (upperName[i] != swappedName[i]) {
    final += upperName[i];
  } else {
    final += swappedName[i].toLowerCase();
  }
}
console.log(final);
```
###### Assignment 1.7
```
let start = 0;
let mix = [1, 2, 3, "A", "B", "C", 4];

for (let i = start; i < mix.length; i++) {
  if (typeof mix[i] === "number" && i != start) {
    console.log(mix[i]);
  }
}
```

<br>

###### Assignment 2.1
```
let friends = ["Ahmed", "Sayed", "Ali", 1, 2, "Mahmoud", "Amany"];
let index = 0;
let counter = 0;

while (index < friends.length) {
  if (
    friends[index].toString().startsWith("A") ||
    typeof friends[index] === "number"
  ) {
    index++;
    continue;
  } else console.log(`${++counter} => ${friends[index]}`);
  index++;
}
```
<hr>

### Week 7: Functions & Scope pt.1  - from 57 to 63

###### Assignment 1
```
function sayHello(theName, theGender = "N/A") {
  switch (theGender) {
    case "Male":
      console.log(`Hello Mr ${theName}`);
      break;
    case "Female":
      console.log(`Hello Mrs ${theName}`);
      break;
    default:
      console.log(`Hello ${theName}`);
  }
}
sayHello("Osama", "Male");
sayHello("Eman", "Female");
sayHello("Sameh");
```
###### Assignment 2
```
function calculate(firstNum, secondNum, operation) {
  if (secondNum === undefined) return console.log(`Second Number Not Found`);
  switch (operation) {
    case "add":
    default:
      console.log(firstNum + secondNum);
      break;
    case "subtract":
      console.log(firstNum - secondNum);
      break;
    case "multiply":
      console.log(firstNum * secondNum);
      break;
  }
}

calculate(20);
calculate(20, 30);
calculate(20, 30, "add");
calculate(20, 30, "subtract");
calculate(20, 30, "multiply");
```
###### Assignment 3
```
function ageInTime(theAge) {
  if (theAge > 100 || theAge < 10) return `Age out of range`;
  console.log(
    `You age is ${theAge} Years or ${theAge * 12} Months or ${
      theAge * 12 * 4.34524
    } Weeks or ${theAge * 365} Days or ${theAge * 8760} Hours or ${
      theAge * 525600
    } Minutes or ${theAge * 3.154e7} Seconds`
  );
}

ageInTime(110);
ageInTime(38);
```
###### Assignment 4
```
function checkStatus(a, b, c) {
  let arr = [a, b, c];
  for (let i = 0; i < arr.length; i++) {
    typeof arr[i] === "string"
      ? (a = arr[i])
      : typeof arr[i] === "number"
      ? (b = arr[i])
      : typeof arr[i] == "boolean"
      ? (c = `You Are Available For Hire`)
      : (c = `You Are Available For Hire`);
  }
  console.log(`Hello ${a}, Your Age Is ${b}, ${c}`);
}

checkStatus("Osama", 38, true);
checkStatus(38, "Osama", true);
checkStatus(true, 38, "Osama");
checkStatus(false, "Osama", 38);
```
###### Assignment 5
```
function createSelectBox(startYear, endYear) {
  document.write(`<select>`);
  for (let i = startYear; i <= endYear; i++) {
    document.write(`<option value="${i}">${i}</option>`);
  }
  document.write(`</select>`);
}
createSelectBox(2000, 2021);
```
###### Assignment 6
```
function multiply(...numbers) {
  let result = 1;
  for (let i = 0; i < numbers.length; i++) {
    if (typeof numbers[i] !== "number") continue;
    result *= parseInt(numbers[i]);
  }
  console.log(result);
}

multiply(10, 20);
multiply("A", 10, 30);
multiply(100.5, 10, "B");
```
<hr>

### Week 8: Functions & Scope pt.2  - from 64 to 70
> To be added

### Higher Order Functions And Practice
> To be added


### Objects
> To be added

