# JavaScript Variable Declarations: let, const, and var
## Differences between let, const, and var
# 1. var
- **Global or Function Scoped:** variables declared with var are global or functional scoped, meaning the scope is global when var variable is declared outside a function or scope is function when it is declared within a function.
- example: [global-function-scope-example](https://www.freecodecamp.org/news/scope-in-javascript-global-vs-local-vs-block-scope/)
```ruby
#variables declared in global scope
var globalVariable = "I'm in global scope."
function myFunction () {

  #this function can access globalVariable
  console.log(globalVariable);

myFunction();

#variables declared in local scope
function myFunction () {
  var localVariable = "I'm in local scope."
  console.log(lovalVariable);
}

myFunction();
```
- **Update and re-declare:** var variables can be updated and redeclared within the same scope.
```ruby
var x = 15;
#re-declare the var variable
var x = 28;
#update var variable
x = 02;
console.log(x);
```
- **Hoisting:** var is hoisted to the top of their scope before code execution.
```ruby
console.log (name);
var name = "isha";
```
- **Declaration and initialization:** it can be declare without initialization and it can be accessed without initialization as its default value is "undefined."
```ruby
#declare without initialization
var x;
console.log(x);

#can be accessed without initialization
console.log(x);
var x = 20;
console.log(x);
```

# 2. let
- **Block Scope:** variables declared with let is a block scoped, meaning it is only accessible within the block{} where it is declared.
```ruby
{
let num = 02;
#calling the function inside the block
console.log(num)
}
```
- **Update but no re-declared:** a variable declared with let can be updated within its scope but cannot be re-declared.
```ruby
let name = "isha";
name = "isha"; #updating a variable declared with let
console.log(name);
```
```ruby
#re-declaring a variable
let name = "isha";
let name = "mae"; #error: Identifier 'name' has already been declared
console.log(name);
```
- **Hoisting:** let are hoisted but stay in the temporal dead zone (tdz) until the initialization.
```ruby
console.log(name);
let name = "isha";
```
- **Declaration and initialization:** it can be declared without initialization but it cannot be accessed without initialization otherwise it will give 'referenceError'.
```ruby
#declare without initialization
let x;
console.log(x(;

#cannot be accessed without initilization
console.log(x);
let x = 13;
console.log(x);
```

# 3. const
- **Block scope:** variables declared with let is a block scoped, meaning it is only accessible within the block{} where it is declared.
```ruby
{
  const num = 2;
  console.log(num);
}
```
- **Neither updated or re-declared:** this means that the value of a variable declared with const remains the same within its scope.
- **Hoisting:** const are hoisted to the top but stays in the temporal dead zone (tdz) until the initialization.
- **Declaration and initialization:** it cannot be accessed without initialization as it cannot be declared without initialization.
- ```ruby
  console.log(num);
  const num = 2;
  console.log(num)
  #ReferenceError: Cannot access 'num' before initialization.

***Reference***

 *freeCodeCamp. (2020, April 2). Var, Let, and Const – What's the Difference? freeCodeCamp.org. https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/*
 
 *GeeksforGeeks. (2024, July 26). JavaScript let. GeeksforGeeks. https://www.geeksforgeeks.org/javascript-let/*
 
 *GeeksforGeeks. (2024b, August 12). Difference between var, let and const keywords in JavaScript. GeeksforGeeks. https://www.geeksforgeeks.org/difference-between-var-let-and-const-keywords-in-javascript/*
 
 *Olawale, A. (2024, September 4). Scope in JavaScript – Global vs Local vs Block Scope Explained. freeCodeCamp.org. https://www.freecodecamp.org/news/scope-in-javascript-global-vs-local-vs-block-scope/*
 
 
