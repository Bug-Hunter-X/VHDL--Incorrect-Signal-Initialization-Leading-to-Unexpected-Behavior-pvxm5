# VHDL: Incorrect Signal Initialization Bug

This repository demonstrates a common but subtle bug in VHDL code: incorrect initialization of internal signals.  Improper initialization can lead to unpredictable behavior during simulation and synthesis.

## Bug Description

The `bug.vhdl` file contains a simple VHDL entity with a process that transfers data from an input to an output. The problem lies in the initialization of the internal signal `internal_data`.  Initializing it to "x"00" might seem correct, but the initial value is crucial, especially if you're modeling a state machine.