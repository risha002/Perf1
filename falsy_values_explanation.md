# Concept of Falsy Values in JavaScript
Falsy values are important in conditional statements and logical operations because they are values that are regarded as false when they are encountered in a boolean environment. JavaScript has six falsy values: undefined, null, NaN, 0, "(empty string)," and false. Falsy values, in contrast to truthy values, stand for "nothingness," "emptiness," or "failure." Because it represents an empty numerical value, the number 0 is false whether it is positive or negative. Similarly, a "" (empty string) is false because it includes no characters, whereas strings with whitespace or content are true. NaN (Not-a-number) is the outcome of invalid or undefined mathematical operations, null represent the intentional absence of any object value, and undefined is a variable that has been declared but not given a value. Understanding falsy values is very important because these are the only values JavaScript treats as false 

## Example:
### 1. null
```javascript
if (false) {
  console.log("hi");
}
//Output: 
```
nothing will be displayed because false is false.

### 2. 0(zero)
```javascript
if (0) { //false 
  console.log("hi");
} else {
  console.log("hello");
}
//Output: "hello"
```
hello will be printed because 0 is false so the else part will be run.

### 3. ""(empty string)
```javascript
if ("") { //false
  console.log("hi");
} else {
  console.log ("hello");
}
//Output: "hello"
```
hello will be printed, but if we remove the else, nothing will be displayed because an empty string is evaluated to be false.
```javascript
if ("") { //false
  console.log("hi");
}
//Output:
```

***Reference***

*GeeksforGeeks. (2024c, December 9). Falsy in JavaScript. GeeksforGeeks. https://www.geeksforgeeks.org/falsy-in-javascript/*

*Falsy - MDN Web Docs Glossary: Definitions of Web-related terms | MDN. (2024, October 25). MDN Web Docs. https://developer.mozilla.org/en-US/docs/Glossary/Falsy*

*Educative. (n.d.). What are falsy values and truthy in JavaScript? https://www.educative.io/answers/what-are-falsy-values-and-truthy-in-javascript*


