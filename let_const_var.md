# JavaScript Variable Declarations: let, const, and var
## Differences between let, const, and var
# 1. var
- **Global or Function Scoped:** var variables are either global or funtional scoped, which means that when they are declared outside of a function, their scope is global, and when they ay declared inside a function, their scope is function.
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
- **Update and re-declare:** within the same scope, var variables can be updated abd re-declared.
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
- **Declaration and initialization:** both declaring and accessing it are possible without initialization because its default value is "undefines."
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
- **Block Scope:** let-declared variables are block scoped, which means they can only be accessed inside the block {} in which they are declared.
```ruby
{
let num = 02;
#calling the function inside the block
console.log(num)
}
```
- **Update but no re-declared:** although it cannot be re-declared, a variable declared with let can be updated within its scope.
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
- **Hoisting:** let are hoisted, but until the initialization they stay in the temporal dead zone (tdz);
```ruby
console.log(name);
let name = "isha";
```
- **Declaration and initialization:** it can be declared without initialization, however if its is not accessed, a 'referenceError' will be displayed.
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
- **Block scope:** const-declared variables are block scope, which means they can only be accessed inside the block {} in which they are defines.
```ruby
{
  const num = 2;
  console.log(num);
}
```
- **Neither updated nor re-declared:** this means that a variable's value stay constant or keeps the same within the scope of a variable declare with const.
- **Hoisting:** const are hoisted to the top, but until initialization, they stays in the temporal dead zone (tdz).
- **Declaration and initialization:** just as it cannot be declared without initialization, it cannot be accesses without initialization either.
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
 
 
