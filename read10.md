# JS Debugging
Errors can (will) happen, every time you write some new computer code.

Programming code might contain syntax errors, or logical errors.

Many of these errors are difficult to diagnose.
Often, when programming code contains errors, nothing will happen. 
There are no error messages, and you will get no indications where to search for errors.
Searching for (and fixing) errors in programming code is called code debugging.
Normally, otherwise follow the steps at the bottom of this page, you activate debugging
in your browser with the F12 key, and select "Console" in the debugger menu.

## ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run .

## EXECUT.ION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 


## Setting Breakpoints
In the debugger window, you can set breakpoints in the JavaScript code.

At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.

After examining values, you can resume the execution of code (typically with a play button).

## The debugger Keyword
The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function.

This has the same function as setting a breakpoint in the debugger.

If no debugging is available, the debugger statement has no effect.

With the debugger turned on, this code will stop executing before it executes the third line.

## Did You Know?
> Debugging is the process of testing, finding, and reducing bugs (errors) in computer programs.
> The first known computer bug was a real bug (an insect) stuck in the electronics.
_________________________________________________________________________________________________________________
> The console helps narrow down the area in which the
> error is located, so you can try to find the exact error.

> JavaScript has 7 different types of errors. Each creates
> its own error object, which can tell you its line number
> and gives a description of the error.

> If you know that you may get an error, you can handle
> it gracefully using the try, catch, finally statements.
> Use them to give your users helpful feedback. 


