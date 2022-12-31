# Single cycle code from on Harris and Harris second edition

This code is taken from Digital Design and Computer Architecture by Harris and Harris.  
Please give enough time understanding how it workds.  

## What's up to be done with this repo?

Three changes should be made to the code in this repo:
1. Implementing the `lb` instruction. It is an I-type instruction which is the same as `lw` but it stores the first byte seen on the given address. The Opcode for this instruction is `100000`.
2. Implementing the `jr` instruction. This instruction loads the `$ra`  into `$pc`. It's an `r-type` instruction. The Opcode and funct for this instruction in order are `000000` and `001000`.
3. Implementing the `jalr` instruction. This instruction is the same as 2 in addition of storing the address of the next instruction in `$ra`. It's an `r-type` instruction. The Opcode and funct for this instruction in order are `000000` and `001001`.
After all the resulting architecture must be impelemented using either `verilog` or `system-verilog`.

## What are the advantages and disadvantages of the `system-verilog`?

It's definitely easier to code using `system-verilog`, *but* it is not fully supported by `iverilog` compiler. Hence if you want to use `iverilog` as you tool in this project, you have to change the given code to `verilog`.  

## How to test the code?

There is a test bench file named `testbench.sv` and a file `memfile.dat` which holds the program to be tested. The assembly program which is equivalent of the machine codes written in `memfile.dat` is in the file `instructions.txt`. Consider reading `testbench.sv` and `instructions.txt` in order to figure out how the testing is going on.


### Have fun and do not cheat
