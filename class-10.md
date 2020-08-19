# Error Handling & Debugging (JS - Chapter 10)

- Order of Execution: To find the source of an error, it helps to know how many scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

- Execution Contexts: The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.

- The Stack: The JavaScript interpreter processes one line of code at a time. When a statement needs data from another function, it stacks (or piles) the new function on top of the current task. 

- Execution Context and Hoisting: Each time a script enters a new execution context, there are two phases of activity: 
  1. Prepare 
  1. Execute 

- Understanding scope: In the interpreter, each execution context has its own variables object. It holds the variables, functions, ans parameters within it. Each execution context can also access its parents variables object. 

- Understanding Errors: If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception handling code. 

- Error Objects: Error objects can help you find where your mistakes are and browsers have tools to help you read them. 

- Types of Error Objects: 
  - SyntaxError
  - ReferenceError
  - TypeError
  - RangeError
  - EvalError
  - URIError
  - Error 
  - NaN

- How to deal with Errors: Now that you know what an error is, and how the browser treats them, there are two things you can do with errors:
  - Debug the script to fix errors 
  - Handle errors gracefully

- A Debugging Workflow: Debugging is about deduction: eliminating potential causes of an error. 
  - Where is the problem?
    - Look at the error message, it tells you:
      - Relevant script
      - The line number
      - Type of error
    - Check how far the script is running
    - Use breakpoints where things are going wrong
  - What is the problem?
    - When you have set breakpoints, you can see the variable around them have the values that you would expect to see.
    - Test parts of the code:
      - Use the console 
      - Call functions
      - Check if objects exits and have the methods that you expect them to.

- Browser DEV Tools and the JavaScript Console: The console will tell you when there is a problem with the script, where to look for the problem, and what kind of issue it seems to be. All browsers have tools (pp. 464-469).

- Writing from the script to the console: Browsers that have a console have a console object, which has several methods that your script can use to display data in the console. The object is documented in the console API. 
  - console.log: Write several values at a time.
  - console.info: General information 
  - console.warn: Warnings 
  - console.error: Hole errors
  - console.table: Output a table that shows:
    - objects
    - arrays 
  - console.assert: test of a condition is met.

- Breakpoints: You can pause the execution of a script on any line by using breakpoints. If you use multiple breakpoints, you can step through them one by one to see where values change and a problem might occur.

- Handling Exceptions: If you know your code might fail, use try, catch and finally. Each one is given its own block of code. 
  - TRY: Specify the code that you think might throw an exception.
  - CATCH: If the TRY throws an exception, CATCH steps in with an alternate line of code.
  - FINALLY: Will run either way.

- DEBUGGING TIPS and COMMON ERRORS - pp. 484-485

- Summary: 
  - If you understand execution context( which have two stages), and stacks, you are more likely to find the error in your code. 
  - Debugging is the process of finding errors. It involves a process of deduction. 
  - The console helps narrow down the area in which the error is located, so you can try to find the exact error. 
  - JavaScript has 7 different types of errors. Each creates its own error object, which can tell you it's line number and gives a description of the error. 
  - If you know that you might get an error, you can handle it gracefully using the TRY, CATHC, FINALLY statements. Use them to give your users helpful feedback. 



