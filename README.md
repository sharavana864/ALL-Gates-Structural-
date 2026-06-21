# Verilog Logic Gates Using Structural Modeling

A Verilog HDL project implementing basic logic gates using **Structural Modeling**. The designs are simulated using **Icarus Verilog (iverilog)** and verified through waveform analysis in **GTKWave**.

## 📌 Project Overview

This repository demonstrates the implementation of fundamental digital logic gates using Verilog's built-in gate primitives. Each gate is designed using structural modeling, tested with a dedicated testbench, and verified through simulation waveforms.

## 🛠️ Tools Used

- Verilog HDL
- Icarus Verilog (iverilog)
- GTKWave
- Visual Studio Code
- Git & GitHub

## 📂 Gates Implemented

- AND Gate
- OR Gate
- NOT Gate
- NAND Gate
- NOR Gate
- XOR Gate
- XNOR Gate

## 📁 Repository Structure

```text
ALL_Gates(Structural)/
│
├── and/
│   ├── and_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── nand/
│   ├── nand_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── nor/
│   ├── nor_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── not/
│   ├── not_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── or/
│   ├── or_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── xor/
│   ├── xor_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── xnor/
│   ├── xnor_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
└── README.md
```

## 🏗️ Structural Modeling Example

Example of an AND gate using structural modeling:

```verilog
module and_gate(
    input a,
    input b,
    output y
);

and(y, a, b);

endmodule
```

In structural modeling, circuits are built by connecting gate primitives such as:

- and
- or
- not
- nand
- nor
- xor
- xnor

## ▶️ Running Simulations

### AND Gate

```bash
cd and
iverilog -o sim and_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### NAND Gate

```bash
cd nand
iverilog -o sim nand_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### NOR Gate

```bash
cd nor
iverilog -o sim nor_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### NOT Gate

```bash
cd not
iverilog -o sim not_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### OR Gate

```bash
cd or
iverilog -o sim or_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### XOR Gate

```bash
cd xor
iverilog -o sim xor_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### XNOR Gate

```bash
cd xnor
iverilog -o sim xnor_gate.v tb.v
vvp sim
gtkwave output.vcd
```

## 📊 Verification

Each testbench:

- Applies all possible input combinations
- Monitors outputs using `$monitor`
- Generates waveform files (`output.vcd`)
- Verifies functionality through GTKWave

## 🎯 Learning Outcomes

- Understanding Structural Modeling in Verilog
- Using Gate Primitives
- Creating Testbenches
- Functional Verification
- Simulation with Icarus Verilog
- Waveform Analysis with GTKWave
- GitHub Repository Management

## 🚀 Clone Repository

```bash
git clone https://github.com/your-username/ALL_Gates-Structural.git
cd ALL_Gates-Structural
```

## 👨‍💻 Author

**Sharavana Kumar**  
B.E. Electronics Engineering (VLSI Design and Technology)  
Rajalakshmi Institute of Technology, Chennai

---

⭐ If you found this project useful, consider giving it a star.
