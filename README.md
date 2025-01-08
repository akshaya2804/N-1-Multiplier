N:1 Multiplexer in Verilog

This repository contains the Verilog implementation of an N:1 Multiplexer along with its testbench. The design is parameterized, allowing you to configure both the number of inputs (N) and the width of each input.

Features

Parameterizable Design: Easily adjust the number of inputs (N) and the bit-width of each input (WIDTH).
Compact and Efficient Code: Implements a simple and effective RTL design using slicing.
Self-checking Testbench: The testbench demonstrates the functionality of the multiplexer.

Design Description

Module: n_to_1_mux
The n_to_1_mux module selects one of the N inputs based on the sel signal and outputs the selected value.

Parameters

N: Number of inputs to the multiplexer.
WIDTH: Bit-width of each input.
Ports
in: Input signal (a concatenated vector of N inputs, each of WIDTH bits).
sel: Select signal (log2(N) bits).
out: Output signal (selected input of WIDTH bits).

Testbench Description

Module: tb_n_to_1_mux
The testbench verifies the functionality of the n_to_1_mux module by:

Initializing the inputs with unique values.
Iterating over all possible values of the sel signal.
Displaying the selected output for each sel value.
