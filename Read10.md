### Call stack ?
a mechanism to keep track of the function calls.

The call stack keeps track of functions to be executed. When we call a function, it’s added, or pushed to the top of the call stack. When the function returns, it’s removed, or popped from the call stack. Any asynchronous functions (fetch, setTimeout, async, etc.) 
are moved to the event queue (more on that later).

### call stack are:
1.  single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

### Types of error messages :
• Reference errors
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

• Syntax Errors
 also called parsing errors, occur at compile time in traditional programming languages and at interpret time in JavaScript.
 
 • Range Error :  when manipulate an array for example and give us  an invalid length

• Type errors: when the types (number, string and so on) you are trying to use or access are incompatible.

### Debugging
the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools.

#### Tools to avoid runtime errors :
• quokka to evaluate your code as you type

• eslint to make sure your style guide is consistency and it will grab you an error or two along the way and

• type script

#### Conclusion
Being able to read error messages and practising debugging is one of  biggest weapons has a developer, we need to do it frequently and with enough time we  will notice a great decrease in the time you spend on each error that you find along the way. 
