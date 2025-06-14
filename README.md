This repository demonstrates a simple Universal Verification Methodology (UVM) testbench for verifying the behavior of a D Flip-Flop (DFF) using SystemVerilog. It serves as a minimal working example for entry-level ASIC/FPGA verification concepts including agent-based architecture, sequences, coverage, and scoreboard-based checking.

## Key Features
- UVM 1.2-based verification environment.
- DUT: D Flip-Flop with asynchronous reset.
- Structured UVM testbench with:
  - Virtual interface
  - Driver and monitor
  - Scoreboard for result checking
  - Sequence with randomized stimulus
- SystemVerilog assertions for signal correctness.
- Self-checking test with pass/fail status.
- Compatible with QuestaSim / EDA Playground.

## How It Works

- The testbench generates randomized `d` and `rst` signals.
- The driver applies stimulus to the DUT through a virtual interface.
- The monitor captures DUT output and sends it to the scoreboard.
- The scoreboard compares expected vs actual behavior of `q`.
- Assertions and functional coverage are used to ensure correctness.

This project is ideal for:
- Beginners learning UVM structure.
- Demonstrating basic verification skills in interviews.
- Applying testbench methodology to a known simple DUT.
