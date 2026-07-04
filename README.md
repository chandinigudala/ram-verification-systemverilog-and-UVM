# Single Port RAM Verification using SystemVerilog & UVM

> A reusable UVM-based verification environment for validating the functionality of a Single Port RAM using SystemVerilog, following industry-standard Design Verification methodologies.

---

## Overview

This project implements a complete UVM verification environment to verify the functional correctness of a Single Port RAM. The verification environment is designed with reusable UVM components, constrained-random stimulus generation, self-checking mechanisms, functional coverage, and SystemVerilog Assertions (SVA) to ensure reliable and comprehensive verification.

---

## Project Objectives

* Verify Single Port RAM read and write operations
* Validate correct data storage and retrieval
* Detect protocol and functional errors automatically
* Develop a reusable UVM verification environment
* Achieve functional coverage through coverage-driven verification
* Implement assertion-based verification using SVA

---

## Features

* Complete UVM Testbench
* Modular & Reusable Verification Components
* Constrained-Random Test Generation
* Self-Checking Scoreboard
* Reference Model
* Functional Coverage Collection
* SystemVerilog Assertions (SVA)
* Read/Write Operation Verification
* Random Address & Data Testing
* Error Detection and Reporting

---

## Technologies Used

| Technology           | Purpose                            |
| -------------------- | ---------------------------------- |
| SystemVerilog        | RTL & Verification                 |
| UVM                  | Universal Verification Methodology |
| SVA                  | Assertion-Based Verification       |
| Functional Coverage  | Coverage-Driven Verification       |
| QuestaSim / ModelSim | Simulation & Debugging             |

---

## UVM Testbench Architecture

```text
Top Testbench
│
├── Interface
│
├── Test
│
├── Environment
│   ├── RAM Agent
│   │   ├── Sequencer
│   │   ├── Driver
│   │   └── Monitor
│   │
│   ├── Scoreboard
│   ├── Reference Model
│   ├── Coverage Collector
│   └── Assertions (SVA)
│
├── Sequences
│
└── Single Port RAM DUT
```

---

## Repository Structure

```text
Single-Port-RAM-UVM/
│
├── rtl/
├── interface/
├── transaction/
├── sequences/
├── sequencer/
├── driver/
├── monitor/
├── agent/
├── env/
├── scoreboard/
├── reference_model/
├── coverage/
├── assertions/
├── tests/
├── tb/
├── docs/
└── README.md
```

---

## Verification Components

* Interface
* Sequence Item (Transaction)
* Sequences
* Sequencer
* Driver
* Monitor
* Agent
* Environment
* Scoreboard
* Reference Model
* Functional Coverage
* SystemVerilog Assertions (SVA)
* Test Cases
* Top Testbench

---

## Test Scenarios

* Write Operation Verification
* Read Operation Verification
* Consecutive Read Transactions
* Consecutive Write Transactions
* Random Read/Write Operations
* Boundary Address Verification
* Maximum Data Value Verification
* Minimum Data Value Verification
* Reset Verification
* Invalid Access Checks (if applicable)

---

## Verification Flow

```text
Sequence
      │
      ▼
Sequencer
      │
      ▼
Driver
      │
      ▼
RAM Interface
      │
      ▼
Single Port RAM (DUT)
      │
      ▼
Monitor
      │
      ├────────► Scoreboard
      ├────────► Coverage
      └────────► Assertions
```

---

## Simulation

Example simulation commands using QuestaSim/ModelSim:

```tcl
vlib work
vlog *.sv
vsim top_tb
run -all
```

---

## Skills Demonstrated

* SystemVerilog
* UVM
* Design Verification
* Functional Verification
* Constrained-Random Verification
* Assertion-Based Verification (SVA)
* Functional Coverage
* Self-Checking Testbench Development
* Scoreboard Implementation
* Verification Component Reusability
* Waveform Debugging

---

## Future Enhancements

* Memory Initialization Tests
* Memory Stress Testing
* Error Injection
* Backdoor Memory Access
* UVM Register Abstraction Layer (RAL)
* Regression Automation
* Continuous Integration (CI) using GitHub Actions

---

## Author

**Gudala Chandini**

Electronics & Communication Engineering Graduate | VLSI Design Verification Enthusiast

**Areas of Interest**

* ASIC Design Verification
* SystemVerilog
* UVM
* Memory Verification
* AMBA Protocols
* Functional Verification

---

⭐ If you found this project useful, consider giving it a star!


## Author

**Chandini Gudala*
