# Single cycle code from on Harris and Harris second edition

This code is taken from Digital Design and Computer Architecture by Harris and Harris.  
Please give enough time understanding how it workds.  

## What's up to be done with this repo?

The students should first study the pipelined architecture of this processor from the mentioned textbook, then they should change it in such a way that a `sw` coming after an `sw` doesn't stall the pipeline.  
After all the resulting architecture must be impelemented using either `verilog` or `system-verilog`.  

## What are the advantages and disadvantages of the `system-verilog`?

It's definitely easier to code using `system-verilog`, *but* it is not fully supported by `iverilog` compiler. Hence if you want to use `iverilog` as you tool in this project, you have to chnage the given code to `verilog`.  

## What has to be payed attention to?

The students must be able to exactly show how the pipeline performs on lines 18 and 19. To be more precise, they have to show that there's no stall on the instruction on line 19.

### Have fun and do not cheat
