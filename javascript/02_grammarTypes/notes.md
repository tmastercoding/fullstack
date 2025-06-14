# Grammar and Types - JavaScript
## intro:
* source: [MDN Web Docs - Grammar and Types](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types) 
* github: [Github](https://github.com/tmastercoding/fullstack)
* from the full stack dev series
## variable names:
* case-sensitive
* unicode (can use ü)
## instructions:
* statements
* seperated by ;
* not necessary if seperated by lines but recommended
## comments:
* // for one line
* /* */ for multi line
* cannot be nested
## declarations:
* var
  * decalres variable, option for init to value
* let
  * declares block-scoped local variable, option for init to a value
* const
  * declares a block-scoped, read-only variable
  * does not prevent mutations
* destructuring
  * unpack values 

## scopes:
* global scope - default scope for all code in script mode
* module scope - scope for code in module mode
* function scope - scope within a function
* block scope - scope created within a block {} (let and const belong here)

## hoisting:
* var declared variables are hoisted (only declaration)
* can refer to variable anywhere in its scope
* var sttements should be placed as near to the top of function - increase clarity
* functions hoisted both declaration and value
  

## global variables
* web pages -> window, window.variable
* globalThis (in all environments)
  
## data types:
* boolean
* null
* undefined
* number (integer or float)
* BigInt
* string
* symbol
* object

When casting, you don't need to declare it as JavaScript is dynamically typed.

Converts numeric values to strings when using + but else converts strings to numbers

* parseInt() for string to integer
  * radix parameter for number system
  * parseInt("101", 2); returns 5
* parseFloat() for string to float
* Number() or + (unary plus)

## literals
* Array Literals
  * list of zero+ expressions enclosed in []
  * can have empty slots by placing two commas in a row
    * returns undefined when accessed with index
    * ignored when end of list
    * should add undefined though for clarity
* Boolean Literals
  * true or false
* Numeric literals
  * Interger literals in different bases & floating point literals in base 10
  * Integer literals:
    * Written in decimal, hexadecimal, octal or binary
    * leading 0 or 0o indicates octal
    * leading 0x indicates hexadecimal
    * leading 0b indicates binary
    * trailing n suffix indicates BigInt
  * Floating-point literals
    * An unsigned decimal integer
    * Decimal point
    * A fraction
    * An exponent - e followed by an integer
* Object literals
  * List of property names and associated values of an object, enclosed with {}
  * Kind of like Python's dictionary
  * Can be nested
  * Unusual property names must be accessed with [] instead of .
  * Supports various shorthand syntaxes for prototyping, methods, super calls, etc.
* RegExp
  * encased in //
* String literals
  * Inclosed in " or '
  * can call any method's of the String object on a string literal
  * Template literal with `
    * can have literal string creation e.g. '\n'
    * Multiline
    * String interpolation (Python's string formatting) with ${}
  * Tagged templates with a call to a tag function for parsing it
    * e.g. print``
