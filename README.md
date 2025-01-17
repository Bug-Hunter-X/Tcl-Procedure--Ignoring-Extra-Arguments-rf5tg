# Tcl Procedure: Ignoring Extra Arguments

This repository demonstrates a common error in Tcl: passing more arguments to a procedure than it's defined to accept. The extra argument(s) are silently ignored, leading to unexpected behavior. This can be difficult to debug, as there's no immediate error message.  The solution involves carefully checking the number of arguments passed and using techniques like `uplevel` for more flexible argument handling.

## Bug
The `bug.tcl` file shows the erroneous code. The `myproc` procedure only accepts two arguments, but three are passed. The third argument is ignored.

## Solution
The `bugSolution.tcl` file presents a corrected version of the code, demonstrating better argument handling.