# Lab 1: Thirty-One Day Month

VHDL template for ECE 281 [Lab 1](https://usafa-ece.github.io/ece281-book/lab/lab1.html)

Targeted toward Digilent Basys3 in Vivado 2024.

Tested on Windows 10.

## Usage

Clone and cd into the directory.

You should see a `.xpr` file. Open it with Vivado!

## GitHub Actions Testbench

The workflow uses the [setup-ghdl-ci](https://github.com/ghdl/setup-ghdl-ci) GitHub action
to run a *nightly* build of [GHDL](https://ghdl.github.io/ghdl/).

First, the workflow uses GHDL to **analyze** all `.vhd` files in `src/`.

Then it **elaborates** `thirtyOneDayMonth_tb` entity.

Finally, the workflow **runs** the simulation. If successful then it will quietly exit with a `0` code.
If any of the `assert` statements fail then GHDL will cease the simulation and exit with non-zero code; this will also cause the workflow to fail.
Assert statements of other severity levels will be reported, but not fail the workflow.

## Demo
I demoed the circuit board in class with Captain January 
Here is the demo for the baseyBoard:
https://usafa0.sharepoint.com/:v:/r/sites/ECE281/Shared%20Documents/General/Demos/Lab%201/T3/LJ_LAB1_DEMO.mp4?csf=1&web=1&e=9jeLMb


## Documentation Statement
I used my notes from the lesson readings, the textbook, and my previous work on the ICE2 to complete this lab. I also recieved help from C3C Ghafoor and C3C Tran to understand how to correcltly wire the circuit board for this lab. I did not use any other resources for this lab. 
