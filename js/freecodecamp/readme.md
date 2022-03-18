## Basic Javascript


1. 8 Datatypes in JS : undefined, null, Boolean, String, Symbol, BigInt, Object, Number
2. Variable name can start with `$` and `_`, but not with a number
3. When variable declared in Js, datatype is `undefined`. Performing an operation on `undefined` value returns NaN.
4. `let a="Nikita";` - a variable declared with `let` can be declared once only.
5.  A variable declared with `const` has all features of `let` and added feature that the value is `read-only.`
6.  Common practice among developers - Uppercase : immutable values; lowercase/ camelCase : mutable identifiers;
7.  `%` : remainder operator, sometimes incorrectly referred as modulus operator. Similar to modulus, but does not work properly for negative numbers.
8.  `const sheSaid="Nikita said,\"It is all about about persistence\" ";` (\ can be used to escape a quote from its interpreted meaning in JS, and just be used as any string : \ is escape character)
9.  
```
\r	carriage return
\t	tab
\b	word boundary
\f	form feed
```
10. To find length of a string, use `.length` property -> `"Nikita Sharma".length` or `thisIsAString.length`.
11. In JS, `string values are immutable` i.e. they a character cannot be changed by accessing it using square brackets once assigned, but the whole string can be changed. Arrays are mutuable in JS.
12. An array/ object can contain values of different data types as well. `const array=["Nikita",21];
13. Js processed `array [1]` correctly (as `array[1]`) and also `array [1] [2]`, but one should avoid giving these spaces to prevent confusion among the programmers.
14.  `push() on array`
```js
const array=["Dance",1];
array.push(["Music", 4]);
// array = ["Dance",1,["Music",4]];
```
15. We can `pop` elements from array, and `pop()` function when applied on array returns the value being popped. 
```js
const array=["Dance",1];
const valuePopped=array.pop();
console.log(valuePopped);
console.log(array);
```
16. Similary, `array.shift()` to pop the first element of an array. We say it like the `shifted off` value. To add an element at the start of an array, use `unshift()`.
```js
var removedElement=arr.shift();
const array=["Dance",1];
array.unshift("Music");
console.log(array);
```
17. No need to specify the return-type (of value being returned) during function declaration.
```js
function plusOne(num) {
  return num + 1;
}

const answer = plusOne(3);
```
18. Variables defined outside a function-block have a global scope. Those created without `let or const` keyword are considered as `global` variables.
19. Varibales declared within a function, and the parameters have local scope.
20. When local and global variable are both defined with same name, then in the block (where local variable is defined), the local variable takes precedence.
21. When return statement not written, code compiles fine and the returned value is `undefined`.
22. `Type Coercion` : type conversion performed automatically, or implicitly javascript engine. `==` type conversion happens, to check whether the value is same, it is not important that the datatype should be same here.
23. switch-case are tested with strict equality (===)
24. switch case for a range
```js
let result = "";
switch(val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4 alone";
}
```
25. In an object data is accessed using the properties, which is basically the variable-name-to-which-value assigned as a key-value pair. If an object has non-string properties, then js wil typecast it into a string. Unlike array which uses index, in case of an object we mention the key for which value needs to be accessed. To summarize, `objects in js are like a dictionary - key/value pair`.
26. `.` operator and `[]` used to access the values of properties of objects. If the property name contains space, then we use `[]` to access the values.
27.  We can add new properties to js objects the same way we modify them - using `. opertor or []`
28. We can delete properties from objects like `delete ourDog.bark;`.
29. To check if there is a key-value pair in the object for a specific key, we use the `object_name.hasOwnProperty(property_name)` method.
```js
const myObj = {
  top: "hat",
};

myObj.hasOwnProperty("top"); //returns trye
myObj.hasOwnProperty("middle"); // returns false
```
30. `Javascript Object Notation or JSON` is a lightweight data-interchange format. It is a text format that is completely independent of a programming language but uses convention that is similar to C-family of langauges. JSON is built of 2 structures : key/value pair. [To read further abour JSON](https://www.json.org/json-en.html). JSON Types : Strings, Numbers, Booleans, null, Arrays, Objects. `Extension for a json file is .json`. Anything in json is valid javascript, and we can directly copy-paste json code in javascript. In this case though, the data (if it was object in json) will be send as a string - so put `around the json data`. We use `JSON.parse(companies)`, and now we can perform companies[0].names. We can use JSON data to transfer data from client to server, or vice-versa. 
31. Accessing values in nested objects : `ourStorage.cabinet["top drawer"].folder2`
32. [Read it](https://medium.com/@amaliesmidth/javascript-short-circuit-conditionals-6606bdeaa30d)
33. 
