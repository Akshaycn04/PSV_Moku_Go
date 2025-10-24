PSV_Moku_Go

Post-Silicon Validation by Configuring the Moku:Go Board as an ATE Machine

Overview

This project demonstrates Post-Silicon Validation (PSV) using the Moku:Go board configured as an Automated Test Equipment (ATE) system. Two digital logic experiments were performed to validate and characterize IC functionality through automated testing and signal observation.

Experiment 1: Testing the 74LS193 (4-bit Up/Down Counter)

The 74LS193 integrated circuit was tested by applying a set of test vectors through the Moku:Go’s digital output channels. The resulting output signals were captured and analyzed using the Logic Analyzer module of the Moku:Go.

Objective: Verify correct counting behavior (up/down count, load, and clear functions).

Method:

Test vectors representing different input combinations were applied.

Output waveforms were monitored and recorded.

Observation:

The output matched the expected logic behavior for all test vectors.

Verified functional integrity of the 74LS193 IC.

Experiment 2: Stress Testing a 2-Bit Full Adder Circuit

A 2-bit full adder was constructed on a breadboard using the following 74LS series ICs:

74LS86 – XOR gates

74LS08 – AND gates

74LS32 – OR gates

Procedure

Randomized input patterns were generated and applied using the Moku:Go board.

Input frequency was gradually increased to observe timing behavior under stress conditions.

**Results**

At lower frequencies, the circuit produced correct and stable outputs.

Beyond a certain threshold frequency, the outputs began to show functional errors, including undefined (‘X’) states.

This behavior indicates timing violations due to propagation delays in the discrete IC logic network.

Conclusion

The Moku:Go board effectively functioned as a flexible ATE platform for both functional and timing-based validation of digital ICs.

74LS193 validation confirmed correct operation across input vectors.

2-bit full adder stress test highlighted timing limits and signal degradation at higher frequencies.

These experiments demonstrate the feasibility of Post-Silicon Validation workflows using compact and reconfigurable lab instrumentation.

Tools & Components

Hardware: Moku:Go, Breadboard, Jumper Wires

ICs: 74LS193, 74LS86, 74LS08, 74LS32

Software: Moku:Go App / Logic Analyzer & Waveform Generator modules
