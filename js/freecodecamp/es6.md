1. Variable declared with `var` keyword is declared globally, or locally if defined in a function whereas variable declared with `let` keyword are defined by the scope (block, statement, expression).
2. What will be the output ?
```js
var printNumTwo;
for (var i = 0; i < 3; i++) {
  if (i === 2) {
    printNumTwo = function() {
      return i;
    };
  }
}
console.log(printNumTwo());
// 3 or 2 ??
```
3. In above problem, as i was updated when i=2, and the variable i and printNumTwo are both defined globally, so the output is 3.
4. **Objects(including arrays and functions)** defined using `const` are still mutable. `const` just prevents reassignment of the variable identifier. Just using `const` does not protect the data from mutation. To make object immutable - `Object.freeze(obj);`
5. Creating `inline functions` in js - no need to name the function as it will never be called anywhere
```js
const myFunc = function() {
  const myVar = "value";
  return myVar;
}
//   CAN NOW BE WRITTEN AS BELOWS WITH ARROW FUNCTION SYNTAX
const myFunc = () => {
  const myVar = "value";
  return myVar;
}
// IF THERE IS NO FUNCITON BODY, JUST A VALUE BEING RETURNED, THEN IT CAN FURTHER BE REDUCED TO 
const myFunc = () => "value";
```
6. We can pass arguments into arrow functions - `const myConcat = (arr1, arr2) => arr1.concat(arr2);`. ES6 introduces default parameters for functions - `const greeting = (name = "Anonymous") => "Hello " + name;`
7. ES6 also introduces the `rest parameters for function parameters`. It can create functions that can take a variable number of arguments. These arguments are stored in an array, which can be accessed later from inside the function.
```js
function howMany(...args) {
  return "You have passed " + args.length + " arguments.";
}
```
<!-- 8. freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-the-spread-operator-to-evaluate-arrays-in-place - start here. Spread operators. -->
