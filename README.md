# <p align="center">JavaScript Bootcamp Assignments</p>

Current Progress : <p>![1%](https://progress-bar.dev/4/?scale=100&width=1100)</p>

### Introduction - from 1 to 9

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

### Data Types And Variables
> To be added


### Numbers And Strings
> To be added


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

