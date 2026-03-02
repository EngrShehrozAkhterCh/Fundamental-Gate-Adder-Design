# Fundamental-Gate-Adder-Design
Structural Verilog implementation of Half and Full Adders using fundamental gates (NOT, AND, OR) to demonstrate gate-level arithmetic logic.
# Fundamental-Gate-Adder-Design

Structural Verilog implementation of Half and Full Adders using fundamental gates (NOT, AND, OR) to demonstrate gate-level arithmetic logic.

## 📌 Project Overview
In digital design, adders are typically built using XOR gates. This project takes a structural approach by decomposing the XOR operation into its fundamental components: **NOT, AND, and OR** gates. This demonstrates a deep understanding of Boolean algebra and hierarchical Verilog design.



[Image of half adder circuit diagram using only NOT AND and OR gates]


---

## 🛠 Circuit Logic

### 1. Half Adder
To avoid using a single XOR gate, the **Sum** is implemented using the **Sum of Products (SOP)** form:
* **Sum** = $AB' + A'B$
* **Carry** = $AB$

### 2. Full Adder
The Full Adder is constructed hierarchically by cascading two Half Adders:
* **Stage 1:** Adds $A$ and $B$.
* **Stage 2:** Adds the result of Stage 1 to the Carry-in ($C_{in}$).
* **Final Carry:** The result of an **OR** operation between the carry outputs of both stages.



---

## 📂 File Structure
* `src/half_adder.v`: Gate-level implementation using primitives.
* `src/full_adder.v`: Top-level module using HA instantiation.
* `tb/half_adder_tb.v`: Testbench for 2-bit addition.
* `tb/full_adder_tb.v`: Testbench for 3-bit addition (including $C_{in}$).

---

## 🚀 Simulation
This project is compatible with **Icarus Verilog**. To run the simulation locally:

**Compile the Full Adder:**
```bash
iverilog -o fa_sim src/half_adder.v src/full_adder.v tb/full_adder_tb.v
