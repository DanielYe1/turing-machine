# turing-machine
Implementation of a turing-machine using the JFLAP that receives a stack automate, an input for the automate and return if it is accepted or not.

In this project we're using the unary notation, so we use 11 to 2, and 111 to 3 as followed to make the implementation simple.

## States
 * Each state is denotated by a "q" followed by a number in unary notation, except the last one. The first state is denotated by "q1", the last one by "qf".

## Symbols
 * Read symbol:
Denotated by a "a" followed by a number in unary notation, the symbol for epsilon is "e" and the symbol for "?" is "t".

 * Popped symbol:
Denotated by a "p" followed by a number in unary notation. The first value of the stack is "p1".

## Separators
 * We use "#" to separate the transitions in the stack automate. It has to be followed by a "$" and the input value that we'll check.
After the check, the output will be the input followed by a "#f"(not accepted) or "#t"(accepted).

## Examples

input example: p1$q1a1p1p1p11qf$a1a11#a

output example: p1$q1a1p1p1p11qf$a1a11#a#t

*Observation: Our implementation is changing the case of the letters(ex:"a" to "A") and changing values the number "1" to "2" to know where the stack automate is.*
