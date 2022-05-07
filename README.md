# <p id="top" align="center">JavaScript Bootcamp Assignments</p>

Current Progress : <p>![](https://progress-bar.dev/68/?scale=100&width=1100)</p>
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
> To be added

### Week 15: Browser Object Model pt.2 - from 111 to 114
> To be added

### Week 16: Destructuring - from 115 to 122
> To be added

### Week 17: Map And Set - from 123 to 133
> To be added

### Week 18: Regular Expression - from 134 to 146
> To be added

### Week 19: Object Oriented Programming - from 147 to 158
> To be added
