# <p id="top" align="center">JavaScript Bootcamp Assignments</p>

Current Progress : <p>![](https://progress-bar.dev/98/?scale=100&width=1100)</p>

<!---
119 out of 121
-->

<hr>

- ### Table of Contents:
    - [Week 1: Introduction](#week-1-introduction---from-1-to-9)
    - [Week 2: Data Types And Variables](#week-2-data-types-and-variables---from-10-to-17)
    - [Week 3: Operators](#week-3-operators---from-18-to-22)
    - [Week 4: Numbers And Strings](#week-4-numbers-and-strings---from-23-to-30)
    - [Week 5: Control Flow](#week-5-control-flow---from-31-to-39)
    - [Week 6: Arrays](#week-6-arrays---from-40-to-47)
    - [Week 7: Loops](#week-7-loops---from-48-to-56)
    - [Week 8: Functions & Scope pt.1](#week-8-functions--scope-pt1----from-57-to-63)
    - [Week 9: Functions & Scope pt.2](#week-9-functions--scope-pt2----from-64-to-70)
    - [Week 10: Higher Order Functions](#week-10-higher-order-functions-and-practice---from-71-to-78)
    - [Week 11: Objects](#week-11-objects---from-79-to-85)
    - [Week 12: Document Object Model pt.1](#week-12-document-object-model-pt1---from-86-to-93)
    - [Week 13: Document Object Model pt.2](#week-13-document-object-model-pt2---from-94-to-101)
    - [Week 14: Browser Object Model pt.1](#week-14-browser-object-model-pt1---from-102-to-110)
    - [Week 15: Browser Object Model pt.2](#week-15-browser-object-model-pt2---from-111-to-114)
    - [Week 16: Destructuring](#week-16-destructuring---from-115-to-122)
    - [Week 17: Map And Set](#week-17-map-and-set---from-123-to-133)
    - [Week 18: Regular Expression](#week-18-regular-expression---from-134-to-146)
    - [Week 19: Object Oriented Programming](#week-19-object-oriented-programming---from-147-to-158)
    - [Week 20: Date, Generators, Modules](#week-20-date-generators-modules---from-159-to-168)
    - [Week 21: AJAX and JSON](#week-21-ajax-and-json---from-169-to-178)
    - [Week 22: Promise](#week-22-promise---from-179-to-188)
<hr>

### Week 1: Introduction - from 1 to 9

###### Assignment 1
```html
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
```javascript
document.write(`<h1 style="color: blue;
font-size: 80px;
font-weight: bold;
text-align: center;
font-family: Arial">ELZERO</h1>`);
```
###### Assignment 3
```javascript
console.log("%cElzero %cWeb %cSchool", "color:red; font-size:40px", "color:green; font-size:40px; font-weight:bold", "color:white; font-size:40px; background-color:blue")
```
###### Assignment 4
```javascript
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
```javascript
console.table(["ash","roaa","Mohammed","Hamdy"])
```
###### Assignment 6
```javascript
// First method
console.log("Iam In Console");
document.write("Iam In Page");

/* Second method */
console.log("Iam In Console");
document.write("Iam In Page");
```
<hr>

### Week 2: Data Types And Variables - from 10 to 17

###### Assignment 1
```javascript
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
```html
<div id="elzero">object</div>
```
###### Assignment 3
```javascript
console.log("I'm In \n\\\\\nLove \\\\\"\"\" '''\n++ With ++ \n\\\"\"\"\\\"\"\"\n\"\"JavaScript\"\"`")
```
###### Assignment 4
```javascript
console.log("_" + `${a}_${b}`.repeat(4) + "_");
```
<hr>

### Week 3: Operators - from 18 to 22

###### Assignment 1
```javascript
console.log(10 * 20 + (15 % 3) + 190 + 10 - 400)
```
###### Assignment 2
```javascript
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
```javascript
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
```javascript
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
```javascript
console.log(-Number.MIN_SAFE_INTEGER)
```
###### Assignment 1.3
```javascript
console.log(Number.MAX_SAFE_INTEGER.toString().length)
```
###### Assignment 1.4
```javascript
let myVar = "100.56789 Views";

console.log(parseInt(myVar));
console.log(+parseFloat(myVar).toFixed(2)); 
```
###### Assignment 1.5
```javascript
let num = 10;

console.log(Number.isInteger(num) + Number.isInteger(num));
```
###### Assignment 1.6
```javascript
let flt = 10.4;

console.log(Math.trunc(flt));
console.log(Math.floor(flt));
console.log(Math.round(flt));
console.log(parseInt(flt));
console.log(Number(flt.toFixed(0)));
```
###### Assignment 1.7
```javascript
console.log(Math.floor(Math.random()*5) ); 
```
<br>

###### Assignment 2.1
```javascript
let userName = "Elzero";
console.log(userName[0].toLowerCase());
console.log(userName.charAt(0).toLowerCase());
console.log(userName.substring(0, 1).toLowerCase());
console.log(userName.slice(0, 1).toLowerCase());
console.log(userName.substr(0, 1).toLowerCase());
console.log(userName.split("", 1).toString().toLowerCase().repeat(3)); 
```
###### Assignment 2.1
```javascript
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
```javascript
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
```javascript
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
```javascript
let a = 20;
let b = 30;
let c = 10;

console.log(a < b && a > c || a == b); 
console.log(a < b || a != c); 
console.log(!(a == b) && !(a > b) && !(a == c) && !(a < c));
```
<br>

###### Assignment 2.1
```javascript
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
```javascript
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
```javascript
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
```javascript
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
```javascript
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

### Week 6: Arrays - from 40 to 47  

###### Assignment 1
```javascript
let myFriends = ["Ahmed", "Elham", "Osama", "Gamal"];
let num = 3;

// Method 1
console.log(myFriends.slice(0, num)); // ["Ahmed", "Elham", "Osama"];

// Method 2
myFriends.length = num;
console.log(myFriends); // ["Ahmed", "Elham", "Osama"];
```

###### Assignment 2
```javascript
let friends = ["Ahmed", "Eman", "Osama", "Gamal"];
friends.shift();
friends.pop();
console.log(friends); // ["Eman", "Osama"]
```

###### Assignment 3
```javascript
let arrOne = ["C", "D", "X"];
let arrTwo = ["A", "B", "Z"];
let finalArr = [];

finalArr = finalArr.concat(arrOne, arrTwo).sort().reverse();
console.log(finalArr); // ["Z", "X", "D", "C", "B", "A"]
```

###### Assignment 4
```javascript
let website = "Go";
let words = [`${website}ogle`, "Facebook", ["Elzero", "Web", "School"]];

console.log(words[words.length - true][0].toUpperCase().slice(website.length)); 
```
###### Assignment 5
```javascript
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
```javascript
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

### Week 7: Loops - from 48 to 56

###### Assignment 1.1
```javascript
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
```javascript
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
```javascript
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
```javascript
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
```javascript
let friends = ["Ahmed", "Sayed", "Eman", "Mahmoud", "Ameer", "Osama", "Sameh"];
let letter = "a";
let ctn = +false;

for (let i = +false; i < friends.length;i++) {
  if (friends[i].startsWith(letter.toUpperCase())) continue;
  console.log(`${++ctn} => ${friends[i]}`);
}
```
###### Assignment 1.6
```javascript
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
```javascript
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
```javascript
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

### Week 8: Functions & Scope pt.1  - from 57 to 63

###### Assignment 1
```javascript
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
```javascript
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
```javascript
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
```javascript
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
```javascript
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
```javascript
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

### Week 9: Functions & Scope pt.2  - from 64 to 70
###### Assignment 1
```javascript
function getDetails(zName, zAge, zCountry) {
  function namePattern(zName) {
    let names = zName.split(" ");
    return `${names[0]} ${names[1][0].toUpperCase()}.`;
  }
  function ageWithMessage(zAge) {
    return parseInt(zAge);
  }
  function countryTwoLetters(zCountry) {
    return zCountry.slice(0, 2).toUpperCase();
  }
  function fullDetails() {
    return `Hello ${namePattern(zName)}, Your Age Is ${ageWithMessage(
      zAge
    )}, You Live In ${countryTwoLetters(zCountry)}`;
  }
  return fullDetails(); // Do Not Edit This
}

console.log(getDetails("Osama Mohamed", "38 Is My Age", "Egypt"));
console.log(getDetails("Ahmed ali", "32 Is The Age", "Syria"));
```

###### Assignment 2
```javascript
let itsMe = () => `Iam A Normal Function`;
console.log(itsMe());
let urlCreate = (protocol, web, tld) => `${protocol}://www.${web}.${tld}`
console.log(urlCreate("https", "elzero", "org"));
```

###### Assignment 3
```javascript
let checker = (zName) => (status) => (salary) =>
  status === "Available"
    ? `${zName}, My Salary Is ${salary}`
    : `Iam Not Avaialble`;

console.log(checker("Osama")("Available")(4000)); 
console.log(checker("Ahmed")("Not Available")()); 
```

###### Assignment 4
```javascript
function specialMix(...data) {
  let result = 0;
  for (let i = 0; i < data.length; i++) {
    result += parseInt(data[i]) || 0;
  }
  return result === 0 ? `All Is Strings` : result;
}

console.log(specialMix(10, 20, 30));
console.log(specialMix("10Test", "Testing", "20Cool"));
console.log(specialMix("Testing", "10Testing", "40Cool"));
console.log(specialMix("Test", "Cool", "Test"));
```

<hr>

### Week 10: Higher Order Functions And Practice - from 71 to 78
###### Assignment 1
```javascript
let mix = [1, 2, 3, "E", 4, "l", "z", "e", "r", 5, "o"];
let mixed = mix
  .map((el) => (typeof el === "number" ? "" : el))
  .reduce((acc, curr) => `${acc}${curr}`);
console.log(mixed);
```
###### Assignment 2
```javascript
let myString = "EElllzzzzzzzeroo";
let arr = myString
  .split("")
  .filter((el, index, arr) => arr[index] !== arr[index + 1])
  .join("");

console.log(arr);
```
###### Assignment 3
```javascript
let myArray = ["E", "l", "z", ["e", "r"], "o"];
let newArray = myArray
  .map((el) => (Array.isArray(el) ? el.reduce((acc, curr) => acc + curr) : el))
  .join("");
console.log(newArray);
```
###### Assignment 4
```javascript
let numsAndStrings = [1, 10, -10, -20, 5, "A", 3, "B", "C"];
let newNumsAndStrings = numsAndStrings
  .filter((el) => !isNaN(el))
  .map((el) => -el);
// [-1, -10, 10, 20, -5, -3]
console.log(newNumsAndStrings);
```
###### Assignment 5
```javascript
let nums = [2, 12, 11, 5, 10, 1, 99];
let newNums = nums.reduce(
  (acc, curr) => (curr % 2 == 0 ? acc * curr : acc + curr),
  1
);
console.log(newNums);
```
<hr>

### Week 11: Objects - from 79 to 85
###### Assignment 1
```javascript
let member = {
  name: "Elzero",
  age: 38,
  country: "Egypt",
  fullDetails: function () {
    return `My Name Is ${this.name}, My Age Is ${this.age}, I Live in ${this.country}`;
  },
};

console.log(member.name);
console.log(member.age);
console.log(member.country); 
console.log(member.fullDetails());
```

###### Assignment 2
```javascript
// Method One
let objMethodOne = {
  property: "Method One",
};
console.log(objMethodOne.property);

// Method Two
let objMethodTwo = new Object({
  property: "Method Two",
});
console.log(objMethodTwo.property); 

// Method Three
let objMethodThree = Object.assign({
  property: "Method Three",
});
console.log(objMethodThree.property); 

// Method Four
let objMethodFour = Object.create({
  property: "Method Four",
});
console.log(objMethodFour.property);
```

###### Assignment 3
```javascript
let a = 1;

let threeNums = {
  b: 2,
  c: 3,
  d: 4,
};

let twoNums = {
  e: 5,
  f: 6,
};

let finalObject = Object.assign({ a }, threeNums, twoNums);
console.log(finalObject);
```

###### Assignment 4
```javascript
let myFavGames = {
  "Trinity Universe": {
    publisher: "NIS America",
    price: 40,
  },
  "Titan Quest": {
    publisher: "THQ",
    bestThree: {
      one: "Immortal Throne",
      two: "Ragnarök",
      three: "Atlantis",
    },
    price: 50,
  },
  YS: {
    publisher: "Falcom",
    bestThree: {
      one: "Oath in Felghana",
      two: "Ark Of Napishtim",
      three: "origin",
    },
    price: 40,
  },
};


let gameName = [];
for (keys in myFavGames) {
  gameName.push(keys);
}

let gamesLength = gameName.length;

for (let i = 0; i < gamesLength; i++) {
  console.log(`The Game Name Is ${gameName[i]}`);
  console.log(`The Publisher Is ${myFavGames[gameName[i]].publisher}`);
  console.log(`The Price Is ${myFavGames[gameName[i]].price}`);

  if (myFavGames[gameName[i]].hasOwnProperty("bestThree")) {
    console.log("- Game Has Releases");
    console.log(`First => ${myFavGames[gameName[i]].bestThree.one}`);
    console.log(`Second => ${myFavGames[gameName[i]].bestThree.two}`);
    console.log(`Third => ${myFavGames[gameName[i]].bestThree.three}`);
  }
  console.log("#".repeat(30));
}
```
<hr>

### Week 12: Document Object Model pt.1 - from 86 to 93
###### Assignment 1
```javascript
console.log(document.getElementById("elzero"));
console.log(document.getElementsByClassName("element")[0]);
console.log(document.getElementsByTagName("div")[0]);
console.log(document.getElementsByName("js")[0]);
console.log(document.querySelector("#elzero"));
console.log(document.querySelector(".element"));
console.log(document.querySelector("div:first-child"));
console.log(document.querySelector(".element#elzero"));
console.log(document.querySelectorAll("#elzero")[0]);
console.log(document.querySelectorAll(".element")[0]);
console.log(document.querySelectorAll("div:first-child")[0]);
console.log(document.querySelectorAll(".element#elzero")[0]);
console.log(document.body.children[0]);
console.log(document.body.childNodes[1]);
console.log(document.body.firstElementChild);
```

###### Assignment 2
```javascript
let myImages = document.images;
for (let i = 0; i < myImages.length; i++) {
  myImages[i].setAttribute(
    "src",
    "https://elzero.org/wp-content/themes/elzero/imgs/logo.png"
  );
  myImages[i].setAttribute("alt", "Elzero Logo");
  console.log(myImages[i]);
}
document.body.style = "background-color:black"
```

###### Assignment 3
```css
// optional
body {
  display: grid;
  place-content: center;
  height: 100vh;
  overflow: hidden;
}

form {
  padding: 50px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: rgb(231, 231, 231);
  border: 1px solid black;
}

form input {
  height: 30px;
  width: 300px;
  margin-bottom: 15px;
  padding-left: 10px;
  background-color: rgb(230, 228, 228);
}

```
```javascript
let myInput = document.querySelector("[name='dollar']");

let result = document.getElementsByClassName("result")[0];

myInput.oninput = function (e) {
  if (myInput.value < 0) {
  } else {
    let newResult = myInput.value * 15.6;
    result.innerHTML = `{${
      myInput.value || 0
    }} USD Dollar = {${newResult.toFixed(2)}} Egyptian Pound`;
  }
};

```
###### Assignment 4
```javascript
let firstDiv = document.querySelector(".one"),
  secondDiv = document.querySelector(".two");

let temp = firstDiv.textContent;
firstDiv.textContent = secondDiv.textContent;
secondDiv.textContent = `${temp} ${secondDiv.attributes.length}`;

firstDiv.title = firstDiv.classList;
secondDiv.title = secondDiv.classList;

```
###### Assignment 5
```javascript
let images = document.images;
for (let i = 0; i < images.length; i++) {
  if (!images[i].hasAttribute("alt")) {
    images[i].alt = `New`;
  } else {
    images[i].alt = `Old`;
  }
}
```
###### Assignment 6

```css
// optional
body {
  height: calc(100vh - 16px);
}
* {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
form {
  display: grid;
  position: relative;
  width: fit-content;
  top: 20%;
  left: 50%;
  transform: translate(-50%, -50%);
}
input,
select {
  width: 300px;
  height: 40px;
  margin-bottom: 20px;
  background-color: #f9f9fd;
  border: 1px rgba(0, 0, 0, 0.253) solid;
  padding: 5px 10px;
  border-radius: 5px;
}

input:last-of-type {
  background-color: #009197;
  border: none;
  border-radius: 5px;
  color: white;
}
.results {
  display: grid;
  grid-template-columns: 300px 300px 300px;
  gap: 25px;
  text-align: center;
  position: absolute;
  top: 120%;
  left: 50%;
  transform: translateX(-50%);
}
.results .box {
  background-color: #fc5029;
  padding: 12px;
  color: white;
  border-radius: 5px;
}
```

```javascript
let form = document.forms[0];
let numberOfElements = document.querySelector("[name='elements']");
let elementText = document.querySelector("[name='texts']");
let type = document.querySelector("[name='type']");
let resultParent = document.getElementsByClassName("results")[0];
form.onsubmit = function (e) {
  /*
     // this code will delete all child elements
      while (resultParent.firstChild) {
        resultParent.removeChild(resultParent.firstChild);
     }
  */
  // but you can do it easly by this :)
  resultParent.innerHTML = "";

  for (let i = 1; i <= numberOfElements.value; i++) {
    let myDiv = document.createElement(type.value);
    let text = document.createTextNode(elementText.value);
    myDiv.className = `box`;
    myDiv.title = `Element`;
    myDiv.id = `id-${i}`;
    myDiv.appendChild(text);
    resultParent.appendChild(myDiv);
  }

  e.preventDefault();
};
```
<hr>



### Week 13: Document Object Model pt.2 - from 94 to 101
###### Assignment 1
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Learn JavaScript</title>
    <script>
      window.onload = function (e) {
        let el = document.getElementsByClassName("open");
        for (let i = 0; i < el.length; i++) {
          if (el[i].innerHTML == "Elzero") {
            el[i].click();
          }
        }
      };
    </script>
  </head>
  <body>
    <a class="open" href="https://google.com">Google</a>
    <a class="open" href="https://elzero.org">Elzero</a>
    <a class="not" href="https://facebook.com">Facebook</a>
    <a class="linked" href="https://linkedin.com">Elzero</a>
    <!-- <script src="main.js"></script> -->
  </body>
</html>
```
###### Assignment 2
> to be added

###### Assignment 3
```javascript
let el = document.querySelector(".our-element");
el.nextElementSibling.remove();
let div = document.createElement("div");
div.innerHTML = "Start";
div.className = "start";
div.title = "Start Element";
div.setAttribute("data-value", "Start");

el.before(div);

let div2 = div.cloneNode(true);
el.after(div2);
```
###### Assignment 4
```javascript
let el = document.querySelector("div");
console.log(el.lastChild.textContent.trim());
```

###### Assignment 5
```javascript
document.addEventListener("click", function (e) {
  if (e.target.parentElement)
    e.target.parentElement.tagName == "BODY"
      ? console.log(`This is ${e.target.nodeName.toLowerCase()}`)
      : "";
});
```
<hr>

### Week 14: Browser Object Model pt.1 - from 102 to 110

###### Assignment 1
```javascript
let promMSG = prompt("Print Number From .. To .. ", "5-20");
prom = promMSG.split("-");
let start = parseInt(prom[0]);
let end = parseInt(prom[1]);
if (start > end) {
  let temp = start;
  start = end;
  end = temp;
}
for (let i = start; i <= end; i++) {
  console.log(i);
}
```
###### Assignment 2
```html
<div class="pop-up">
      <div class="x">X</div>
      <h1>Welcome</h1>
      <p>Welcome to ash's world!</p>
    </div>
```
```css
body {
  display: grid;
  height: calc(100vh - 16px);
  place-content: center;
}
.pop-up {
  position: relative;
  width: 400px;
  height: 100px;
  padding: 30px;
  border-radius: 7px;
  text-align: center;
  background-color: #F5F3F4;
  transition: 0.3s;
  opacity: 0;
  border: 1px solid rgba(0, 0, 0, 0.075);
}
h1 {
  margin: 0;
  margin-top: 10px;
}
p {
  margin: 0;
  margin-top: 20px;
}
.x {
  position: absolute;
  border-radius: 50%;
  background-color: rgb(255 84 84);
  font-size: 10px;
  width: 30px;
  display: grid;
  color: white;
  height: 30px;
  place-content: center;
  top: -10px;
  right: -10px;
  cursor: pointer;
}
```
```javascript
let popUp = document.getElementsByClassName("pop-up")[0];
setTimeout(() => {
  popUp.style.opacity = 1;
}, 5000);

let after = document.querySelector(".x");

after.addEventListener("click", () => {
  popUp.style.opacity = 0;
});

```
###### Assignment 3
```javascript
let cnt = document.querySelector("div");
setInterval(() => {
  if (cnt.innerHTML == "0") {
    clearInterval(cnt);
  } else {
    cnt.innerHTML -= 1;
  }
}, 1000);
```
###### Assignment 3
```javascript
let cnt = document.querySelector("div");
setInterval(() => {
  if (cnt.innerHTML == "0") {
    location.replace("https://www.google.com");
  } else {
    cnt.innerHTML -= 1;
  }
}, 1000);
```

###### Assignment 4
```javascript
let cnt = document.querySelector("div");
setInterval(() => {
  if (cnt.innerHTML == "0") {
    clearInterval(cnt);
  } else if (cnt.innerHTML == "5") {
    window.open("https://elzero.org", "_blank", "width:400,height:500,top:50,left:300");  
    cnt.innerHTML -= 1;
  } else {
    cnt.innerHTML -= 1;
  }
}, 1000);
```
<hr>

### Week 15: Browser Object Model pt.2 - from 111 to 114

###### Assignment 1
```html
<select name="font" id="font">
    <option value="Cairo">Cairo</option>
    <option value="Open">Open Sans</option>
    <option value="Roboto">Roboto</option>
</select>
<select name="color" id="color">
    <option value="Red">Red</option>
    <option value="Blue">Blue</option>
    <option value="Green">Green</option>
    <option value="Black">Black</option>
    <option value="Pink">Pink</option>
    <option value="Yellow">Yellow</option>
</select>
<select name="size" id="size">
    <option value="16">16px</option>
    <option value="18">18px</option>
    <option value="20">20px</option>
    <option value="22">22px</option>
    <option value="24">24px</option>
    <option value="26">26px</option>
    <option value="28">28px</option>
    <option value="30">30px</option>
</select>
```

```javascript
let selects = document.querySelectorAll("select");
let test = document.querySelector(".test");

if (localStorage.size != 0) {
  document.body.style.fontFamily = localStorage.getItem("font");
  document.body.style.color = localStorage.getItem("color");
  document.body.style.fontSize = `${localStorage.getItem("size")}px`;

  selects[0].value = localStorage.getItem("font");
  selects[1].value = localStorage.getItem("color");
  selects[2].value = localStorage.getItem("size");
}

selects.forEach((select) => {
  select.addEventListener("change", function () {
    let font = selects[0].value;
    let color = selects[1].value;
    let size = selects[2].value;

    localStorage.setItem("font", font);
    localStorage.setItem("color", color);
    localStorage.setItem("size", size);

    document.body.style.fontFamily = localStorage.getItem("font");
    document.body.style.color = localStorage.getItem("color");
    document.body.style.fontSize = `${localStorage.getItem("size")}px`;
  });
});

```
###### Assignment 2

```html
<form>
  <input type="text" name="name" />
  <input type="password" name="password" />
  <input type="email" name="email" />
  <select name="department">
      <option value="IT">Information Technology</option>
      <option value="CS">Computer Science</option>
      <option value="DS">Decision Support</option>
      <option value="AI">Artificial Intelligence</option>
      <option value="IS">Information System</option>
  </select>
</form>
```

```javascript
let input = document.querySelectorAll("input");

let select = document.querySelector('[name="department"]');

select.addEventListener("change", function (e) {
  sessionStorage.setItem("department", e.target.value);
});

select.value = sessionStorage.getItem("department");
input[0].value = sessionStorage.getItem("name");
input[1].value = sessionStorage.getItem("password");
input[2].value = sessionStorage.getItem("email");

let inputs = document.querySelectorAll("input");
inputs.forEach((input) => {
  input.addEventListener("blur", function (e) {
    sessionStorage.setItem(e.target.name, e.target.value);
  });
});
```
<hr>

### Week 16: Destructuring - from 115 to 122

###### Assignment 1
```javascript
let myNumbers = [1, 2, 3, 4, 5];

// Write Your Destructuring Assignment Here
[a, , , , e] = myNumbers;
console.log(a * e); // 5
```

###### Assignment 2
```javascript
let mySkills = ["HTML", "CSS", "JavaScript", ["PHP", "Python", ["Django", "Laravel"]]];

// Write Your Destructuring Assignment Here
[a,b,c,[d,e,[f,g]]] = mySkills;
console.log(`My Skills: ${a}, ${b}, ${c}, ${d}, ${e}, ${f}, ${g}`);

// My Skills: HTML, CSS, JavaScript, PHP, Python, Django, Laravel

```

###### Assignment 3
```javascript
let arr1 = ["Ahmed", "Sameh", "Sayed"];
let arr2 = ["Mohamed", "Gamal", "Amir"];
let arr3 = ["Haytham", "Shady", "Mahmoud"];

// Play With Arrays To Prepare For Destructuring
// Write Your Destructuring Assignment Here
[, a, b, , , , c] = arr3.concat(arr2, arr1);
console.log(`My Best Friends: ${a}, ${b}, ${c}`);

// My Best Friends: Shady, Mahmoud, Ahmed

```


###### Assignment 4
```javascript
const member = {
  age: 30,
  working: false,
  country: "Egypt",
  hobbies: ["Reading", "Swimming", "Programming"],
};

// Write Your Destructuring Assignment Here
let {
  age: a,
  working: w,
  country: c,
  hobbies: [h1, , h3],
} = member;
console.log(`My Age Is ${a} And Iam ${w ? "" : "Not"} Working`);
// My Age Is 30 And Iam Not Working

console.log(`I Live in ${c}`);
// I Live in Egypt

console.log(`My Hobbies: ${h1} And ${h3}`);
// My Hobbies: Reading And Programming

```


###### Assignment 5
```javascript
const game = {
  title: "YS",
  developer: "Falcom",
  releases: {
    "Oath In Felghana": ["USA", "Japan"],
    "Ark Of Napishtim": {
      US: "20 USD",
      JAP: "10 USD",
    },
    Origin: "30 USD",
  },
};

const {
  title: t,
  developer: d,
  releases: {
    "Oath In Felghana": [u, j],
    "Ark Of Napishtim": { US: u_price = "20 USD", JAP: j_price = "10 USD" },
    Origin: or = "30 USD",
  },
} = game;
const [o, a] = Object.keys(game.releases);

// Write Your Destructuring Assignment/s Here

console.log(`My Favourite Games Style Is ${t} Style`);
// My Favourite Games Style Is YS Style

console.log(`And I Love ${d} Games`);
// And I Love Falcom Games

console.log(`My Best Release Is ${o} It Released in ${u} & ${j}`);
// My Best Release Is Oath In Felghana It Released in USA & Japan

console.log(`Although I Love ${a}`);
// Although I Love Ark Of Napishtim

console.log(`${a} Price in USA Is ${u_price}`);
// Ark Of Napishtim Price in USA Is 20 USD

console.log(`${a} Price in Japan Is ${j_price}`);
// Ark Of Napishtim Price in Japan Is 10 USD

console.log(`Origin Price Is ${or}`);
// Origin Price Is 30 USD
```

###### Assignment 6
```javascript
let chosen = 3;

let myFriends = [
  { title: "Osama", age: 39, available: true, skills: ["HTML", "CSS"] },
  { title: "Ahmed", age: 25, available: false, skills: ["Python", "Django"] },
  { title: "Sayed", age: 33, available: true, skills: ["PHP", "Laravel"] },
];

// Write Your Code Here

switch (chosen) {
  case 1:
    ({
      title,
      age,
      available,
      skills: [, skill],
    } = myFriends[0]);
    break;
  case 2:
    ({
      title,
      age,
      available,
      skills: [, skill],
    } = myFriends[1]);
    break;
  case 3:
    ({
      title,
      age,
      available,
      skills: [, skill],
    } = myFriends[2]);
    break;
}

console.log(title, age, available ? "Available" : "Not Available", skill);
```


<hr>


### Week 17: Map And Set - from 123 to 133

###### Assignment 1
```javascript
let setOfNumbers = new Set([10]);
setOfNumbers.add(20).add(setOfNumbers.size);

console.log(setOfNumbers);

console.log([...setOfNumbers].pop());
/* explanation of the above line of code:
    1. the ... operator within the [] brackets is used to convert the whole set into an array
       by the concept of destructuring from previous lessons.
    2. the pop() method is used to remove the last element of the array.
*/
```

###### Assignment 2
```javascript
let myFriends = ["Osama", "Ahmed", "Sayed", "Sayed", "Mahmoud", "Osama"];
console.log(Array.from(new Set(myFriends)).sort());
*/
```


###### Assignment 3
```javascript
let myInfo = {
  username: "Osama",
  role: "Admin",
  country: "Egypt",
};

let myMap = new Map(Object.keys(myInfo).map((key) => [key, myInfo[key]]));
console.log(myMap);
console.log(myMap.size);
console.log(myMap.has("role"));
*/
```

###### Assignment 4
```javascript
let theNumber = 100020003000;
console.log([...new Set(theNumber.toString())].filter((item)=>item!=0).join(""));
```

###### Assignment 5
```javascript
let theName = "Elzero";
console.log([...theName])
console.log(Array(...new Set(theName)))
console.log(theName.split(""))
console.log(Array.from(theName))
console.log(Object.assign([], theName))
```

###### Assignment 6
```javascript
let chars = ["A", "B", "C", 20, "D", "E", 10, 15, 6];

// Move numbers in the first of array
let numbersCount = 0;
chars.forEach(function (char, index, array) {
  if (typeof char === "number") {
    let num = array.splice(index, 1);
    array.unshift(...num);
    numbersCount++;
  }
});

chars.copyWithin(0, numbersCount, 2 * numbersCount);
console.log(chars);
```

###### Assignment 7
```javascript
let numsOne = [1, 2, 3];
let numsTwo = [4, 5, 6];

// Needed Output

// 1st Method
console.log(numsOne.concat(numsTwo));

// 2nd Method
console.log([...numsOne, ...numsTwo]);

// 3rd Method
console.log(
  (merged = numsTwo.reduce((arr, item) => {
    arr.push(item);
    return arr;
  }, numsOne))
);

// 4th Method
numsOne.push(...numsTwo);
console.log(numsOne);

// 5th Method
console.log([...new Set([...numsOne, ...numsTwo])]);
```
<hr>

### Week 18: Regular Expression - from 134 to 146

###### Assignment 1
```javascript
let ip = "2001:db8:3333:4444:5555:6666:7777:8888";
let ipRegex = /^([0-9a-fA-F]{1,4}:){7}[0-9a-fA-F]{1,4}$/;

console.log(ip.match(ipRegex));
```

###### Assignment 2
```javascript
let specialNames = "Os10O OsO Os100O Osa100O Os1000 Os100m";
let specialNamesRegex = /Os(\d+)?O/g;

console.log(specialNames.match(specialRegex));
```

###### Assignment 3
```javascript
let phone = "+(995)-123 (4567)";
let phoneRegex = /\+\(\d{3}\)-\d{3}\s\(\d{4}\)/gi;

console.log(phone.match(phoneRegex));
```

###### Assignment 4
```javascript
let re = /https?:\/\/(?:[-\w]+\.)?([-\w]+)\.\w+(?:\.\w+)?\/?.*/i;


// https? : the '?' means that the character can be optional
// : the ':' means that the character is mandatory
// \/\/ : the '/' character is escaped 
// (?:[-\w]+\.) : the group of characters between the brackets is optional =>  (www.) opt
// ([-\w]+) : the group of characters between the brackets is mandatory =>  (coursera) mandatory
// \. : the '.' character is mandatory
// \w+ : a group of mandatory characters
// (?:\.\w+)? : the group of characters between the brackets is optional =>  (.com) opt
// \/? : the '/' character is optional
// .* : the group of characters between the brackets is mandatory => (/courses/js/index.html) 
```

###### Assignment 5
```javascript
let date1 = "25/10/1982";
let date2 = "25 - 10 - 1982";
let date3 = "25 10 1982";
let date4 = "25 10 82";

let re = /\d{1,2}(\s-\s|\s|\/)\d{1,2}(\s-\s|\s|\/)\d{2,4}/gi;

console.log(date1.match(re)); // "25/10/1982"
console.log(date2.match(re)); // "25 - 10 - 1982"
console.log(date3.match(re)); // "25 10 1982"
console.log(date4.match(re)); // "25 10 82"
```

<hr>

### Week 19: Object Oriented Programming - from 147 to 158
###### Assignment 1
```javascript
class Car {
  constructor(name, model, price) {
    this.name = name;
    this.model = model;
    this.price = price;
  }
  run() {
    return "Car Is Running Now";
  }
  stop() {
    return "Car Is Stopped";
  }
}
// Needed Output

let car1 = new Car("BMW", "X5", 100000);
let car2 = new Car("Audi", "A6", 80000);
let car3 = new Car("Mercedes", "C200", 120000);

console.log(
  `Car One Name Is ${car1.name} And Model Is ${car1.model} And Price Is ${car1.price}`
);
console.log(car1.run());
```

###### Assignment 2
```javascript
class Phone {
  constructor(name, serial, price) {
    this.name = name;
    this.serial = serial;
    this.price = price;
  }
}

class Tablet extends Phone {
  constructor(name, serial, price, size) {
    super(name, serial, price);
    this.size = size;
  }
  fullDetails() {
    return `${this.name} Serial is ${this.serial} And Size is ${
      this.size || "Unknown"
    }`;
  }
}

// Write Tablet Class Here

let TabletOne = new Tablet("iPad", 100200300, 1500, 12.9);
let TabletTwo = new Tablet("Nokia", 350450650, 800, 10.5);
let TabletThree = new Tablet("LG", 250450650, 650);

console.log(`${TabletOne.fullDetails()}`);
// iPad Serial is 100200300 And Size Is 12.9

console.log(`${TabletTwo.fullDetails()}`);
// Nokia Serial is 350450650 And Size Is 10.5

console.log(`${TabletThree.fullDetails()}`);
// LG Serial is 250450650 And Size Is Unknown
```

###### Assignment 3
```javascript
class User {
  #c;
  constructor(username, card) {
    this.u = username;
    this.#c = card;
  }
  validate() {
    // Validate data
    let credit = typeof this.#c === "string" ? this.#c : this.#c.toString();
    let creditRe = /\d{4}/g;
    let result = credit.match(creditRe);
    result = result
      .map((el, i) => {
        return i < result.length - 1 ? (el += "-") : el;
      })
      .join("");

    return result;
  }
  get showData() {
    return `Hello ${this.u} Your Credit Card Number Is ${this.validate()}`;
  }
}

// Do Not Edit Anything Below

let userOne = new User("Osama", "1234-5678-1234-5678");
let userTwo = new User("Ahmed", "1234567812345678");
let userThree = new User("Ghareeb", 1234567812345678);

console.log(userOne.showData);
// Hello Osama Your Credit Card Number Is 1234-5678-1234-5678

console.log(userTwo.showData);
// Hello Ahmed Your Credit Card Number Is 1234-5678-1234-5678

console.log(userThree.showData);
// Hello Ghareeb Your Credit Card Number Is 1234-5678-1234-5678

console.log(userOne.c); // Prevent Accessing To Card Property Here
// Undefined
```

###### Assignment 4
```javascript
String.prototype.addLove = function () {
  return `I Love ${this} Web School`;
};
// Do Not Edit Below
let myStr = "Elzero";
console.log(myStr.addLove()); // I Love Elzero Web School
```

###### Assignment 5
```javascript
const myObj = {
  username: "Elzero",
  id: 100,
  score: 1000,
  country: "Egypt",
};

// Write Your Code Here
Object.defineProperties(myObj, {
  id: {
    enumerable: false,
  },
  score: {
    writable: false,
  },
});
delete myObj.country;

myObj.score = 500;

for (let prop in myObj) {
  console.log(`${prop} => ${myObj[prop]}`);
}

console.log(myObj);

// Needed Output

// "username => Elzero"
// "score => 1000"
// {username: 'Elzero', score: 1000, id: 100}
```

### Week 20: Date Generators Modules - from 159 to 168 
###### Assignment 1
```javascript
let date = new Date("27 feb 2002");
let confDate = Date.now() - date.getTime();
console.log(`${(confDate /= 1000)} Seconds`);
console.log(`${(confDate /= 60)} Minutes`);
console.log(`${(confDate /= 60)} Hours`);
console.log(`${(confDate /= 24)} Days`);
console.log(`${(confDate /= 30)} Months`);
console.log(`${(confDate /= 12)} Years`);

```
###### Assignment 2
```javascript
let tenYearsAfterOrigins = new Date(0);
tenYearsAfterOrigins.setFullYear(1980, 0, 1);
tenYearsAfterOrigins.setHours(0, 0, 1, 0);
console.log(tenYearsAfterOrigins);
```
###### Assignment 3
```javascript
let date = new Date();
date.setDate(-1);

// Needed Output

// "Sat Apr 30 2022 18:13:20 GMT+0200 (Eastern European Standard Time)"
// "Previous Month Is April And Last Day Is 30"

console.log(date);

console.log(
  `Previous Month Is ${date.toLocaleString("en-us", {
    month: "long",
  })} And Last Day Is ${date.getDate()}`
);
```
###### Assignment 4
```javascript
// First Method
let BirthDate1 = new Date(2002, 1, 27, 0, 0, 0, 0);
console.log(BirthDate1);

// Second Method
let BirthDate2 = new Date("2002/02/27");
console.log(BirthDate2);

// Third Method
let BirthDate3 = new Date(Date.parse("2002/02/27"));
console.log(BirthDate3);
```
###### Assignment 5
```javascript
let t1 = performance.now();
for (let i = 1; i < 100000; i++) {
  console.log(i);
}
let t2 = performance.now();

console.log(`Loop Took ${Math.trunc(t2 - t1)} milliseconds`);
```
###### Assignment 6
```javascript
// Write Your Generator Function Here
function* gen() {
  let i = 1;
  while (true) {
    yield 2 * (50 * Math.pow(i, 2) - 80 * i + 37);
    i++;
  }
}
let generator = gen();

console.log(generator.next()); // {value: 14, done: false}
console.log(generator.next()); // {value: 154, done: false}
console.log(generator.next()); // {value: 494, done: false}
console.log(generator.next()); // {value: 1034, done: false}
console.log(generator.next()); // {value: 1774, done: false}
console.log(generator.next()); // {value: 2714, done: false}
console.log(generator.next()); // {value: 3854, done: false}
console.log(generator.next()); // {value: 5194, done: false}
console.log(generator.next()); // {value: 6734, done: false}

// The mathimatical equation is 2(50n^2 - 80n + 37) solved by : https://www.wolframalpha.com/widgets/view.jsp?id=a3af2e675c3bfae0f2ecce820c2bef43
```
###### Assignment 7
```javascript
function* genNumbers() {
  yield* [1, 2, 2, 2, 3, 4, 5];
}
function* genLetters() {
  yield* ["A", "B", "B", "B", "C", "D"];
}

// Write Your Generator Function Here
function* genAll() {
  yield* new Set(genNumbers());
  yield* new Set(genLetters());
}
let generator = genAll();

console.log(generator.next()); // {value: 1, done: false}
console.log(generator.next()); // {value: 2, done: false}
console.log(generator.next()); // {value: 3, done: false}
console.log(generator.next()); // {value: 4, done: false}
console.log(generator.next()); // {value: 5, done: false}
console.log(generator.next()); // {value: "A", done: false}
console.log(generator.next()); // {value: "B", done: false}
console.log(generator.next()); // {value: "C", done: false}
console.log(generator.next()); // {value: "D", done: false}

```

###### Assignment 8
```javascript
// main.js file

import calc, * as modOne from "./mod-one.js";

console.log(calc(modOne.numOne, modOne.numTwo, modOne.numThree)); // 60

// mod-one.js File
import { numOne, numTwo, numThree } from "./mod-two.js";
export default function (a, b, c) {
  return a + b + c;
}
export { numOne, numTwo, numThree };

// mod-two.js File
let a = 10; // Do Not Edit Names
let b = 20; // Do Not Edit Names
let c = 30; // Do Not Edit Names

export { a as numOne, b as numTwo, c as numThree };
```

<hr>

### Week 21: AJAX and JSON - from 169 to 178
###### Assignment 1
```json
[
  {
    "id": "1",
    "author": "Ash",
    "title": "Why Ash is the best Pokemon",
    "category": "Games",
    "content": "lorem ipsum dolor sit amet"
  },
  {
    "id": "2",
    "author": "Hamdy",
    "title": "Benfits of eating carrots",
    "category": "Food",
    "content": "lorem ipsum dolor sit amet"
  },
  {
    "id": "3",
    "author": "Salma",
    "title": "How to make a good salad",
    "category": "Food",
    "content": "lorem ipsum dolor sit amet"
  },
  {
    "id": "4",
    "author": "Mariam",
    "title": "Javascript is weird",
    "category": "Javascript",
    "content": "lorem ipsum dolor sit amet"
  },
  {
    "id": "5",
    "author": "Mahdy",
    "title": "Tips for life",
    "category": "All",
    "content": "lorem ipsum dolor sit amet"
  }
]
```
###### Assignment 2
```javascript
let req = new XMLHttpRequest();
req.open("GET", "articles.json");
req.send();
req.onreadystatechange = function () {
  if (req.readyState === 4 && req.status === 200) {
    let articles = JSON.parse(req.responseText);
    for (article of articles) {
      console.log(article);
    }
   console.log(`Data Loaded`);
  }
};
```

###### Assignment 3
```javascript
let req = new XMLHttpRequest();
req.open("GET", "articles.json");
req.send();
req.onreadystatechange = function () {
  if (req.readyState === 4 && req.status === 200) {
    let mainData = JSON.parse(req.responseText);
    for (article of mainData) {
      article.category = "All";
    }

    console.log(mainData);
    updatedData = JSON.stringify(mainData);
    console.log(updatedData);
    console.log(`Data Loaded`);
  }
};
```

###### Assignment 4
```javascript
let req = new XMLHttpRequest();
req.open("GET", "articles.json");
req.send();
req.onreadystatechange = function () {
  if (req.readyState === 4 && req.status === 200) {
    let mainData = JSON.parse(req.responseText);
    let articlesDiv = document.createElement("div");
    articlesDiv.id = "data";
    for (article of mainData) {
      let articleDiv = document.createElement("div");
      let articleTitle = document.createElement("h2");
      articleTitle.innerHTML = article.title;
      let articleContent = document.createElement("p");
      articleContent.innerHTML = article.content;
      let articleAuthor = document.createElement("p");
      articleAuthor.innerHTML = article.author;
      let articleCategory = document.createElement("p");
      articleCategory.innerHTML = article.category;

      articleDiv.appendChild(articleTitle);
      articleDiv.appendChild(articleContent);
      articleDiv.appendChild(articleAuthor);
      articleDiv.appendChild(articleCategory);

      articlesDiv.appendChild(articleDiv);
    }
    document.body.appendChild(articlesDiv);
  }
};
```
<hr>


### Week 22: Promise - from 179 to 188
###### Assignment 1
```javascript
let myPromise = new Promise(function (myResolve, myReject) {
  let request = new XMLHttpRequest();
  request.onload = function () {
    if (request.status === 200) {
      let myData = JSON.parse(request.responseText);
      myData.length = 5;
      myResolve(myData);
    } else {
      myReject("Error");
    }
  };
  request.open("GET", "articles.json");
  request.send();
});

myPromise.then((domData) => {
  for (let i = 0; i < domData.length; i++) {
    let myDiv = document.createElement("div");
    let myH3 = document.createElement("h3");
    let myP = document.createElement("p");
    myH3.innerText = domData[i].title;
    myP.innerText = domData[i].description;
    myDiv.appendChild(myH3);
    myDiv.appendChild(myP);
    document.body.append(myDiv);
  }
});

```

###### Assignment 2
```javascript
async function fetchAPI() {
  try {
    let response = await fetch("articles.json");
    let myData = await response.json();
    myData.length = 5;
    return myData;
  } catch (err) {
    console.log(err);
  }
}

fetchAPI().then((domData) => {
  for (data of domData) {
    let myDiv = document.createElement("div");
    let myH3 = document.createElement("h3");
    let myP = document.createElement("p");
    myH3.innerText = data.title;
    myP.innerText = data.description;
    myDiv.appendChild(myH3);
    myDiv.appendChild(myP);
    document.body.append(myDiv);
  }
```
