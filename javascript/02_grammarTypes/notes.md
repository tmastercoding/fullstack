# basics
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

