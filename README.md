# VHDL Counter with Overflow Handling
This repository demonstrates a common VHDL coding error related to counter overflow and provides a corrected version.

## Bug Description:
The original `buggy_counter.vhd` contains a potential issue in how the counter handles overflow. When the counter reaches its maximum value (15), it resets to 0. However, depending on the synthesis tool and target hardware, this might not produce the intended behavior or lead to unexpected delays. 

## Solution:
The `fixed_counter.vhd` provides a corrected version which uses the modulo operator for a more explicit and generally better-synthesized counter reset.

## How to Use:
1. Clone the repository.
2. Simulate or synthesize both versions using your preferred VHDL tools (e.g., ModelSim, Vivado).
3. Compare the results to observe the difference in behavior.