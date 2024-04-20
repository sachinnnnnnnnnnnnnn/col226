
About Assignment 

1.Expression (exp) type: 

This defines the syntax of expressions in the language. 

It includes variables, abstraction (lambda), application, numerals, booleans, tuples, projection, conditional expression (if-then-else), and various arithmetic and logical operations.


2.Value type: 

This defines the possible values that expressions can evaluate to. It includes numbers, booleans, tuples, and closures.


3.Opcode type: 

This represents the instructions for the SECD machine. 

It includes operations like lookup, application, creating closures, returning from a function call, constants, arithmetic, logical operations, projection, and conditional branching.

4.Compilation function (compile_exp):

This function translates expressions in the language into sequences of opcodes for the SECD machine.

5.Execution function (execute_secd):

This function interprets the sequences of opcodes produced by the compiler.

It maintains an environment (association list of variable bindings), a stack for operand values, a dump for storing continuation frames during function calls, and the code being executed. 

It pattern matches on each opcode and performs the corresponding operation.


6.Top-level SECD function (secd): 


This function provides a convenient interface for executing SECD code. It takes an initial environment, stack, code, and dump as arguments and calls the execute_secd function with these arguments.
7.Example executions: 
These are calls to execute_secd with different expressions to test the SECD machine.
