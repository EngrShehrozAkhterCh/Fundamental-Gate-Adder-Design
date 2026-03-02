# Half Adder & Full Adder – Digital Systems Lab

## 📌 Overview
This project demonstrates the design and implementation of a **Half Adder** and a **Full Adder** using only basic logic gates (**NOT, AND, OR**).

XOR gates were intentionally not used directly in order to strengthen understanding of fundamental digital logic concepts and gate-level design.

---

## ⚙️ Implementation

### Half Adder
- **Sum** = A ⊕ B  
- **Carry** = A · B  

---

### Full Adder (Using Two Half Adders)

A Full Adder is implemented by cascading two Half Adders:

#### 1️⃣ First Half Adder (Inputs: A, B)
- Sum₁ = A ⊕ B  
- Carry₁ = A · B  

#### 2️⃣ Second Half Adder (Inputs: Sum₁, Cin)
- Sum = Sum₁ ⊕ Cin  
- Carry₂ = Sum₁ · Cin  

#### ✅ Final Carry Output


---

## 📊 Truth Tables

### Half Adder

| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

---

### Full Adder

| A | B | Cin | Sum | Carry |
|---|---|-----|-----|-------|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

---

## 👥 Team Members
- Muhammad Shehroz Akhter  
- Ziaullah 
- Abdullah  

---

## 🧠 Learning Outcomes
- Understanding Boolean algebra implementation
- Designing arithmetic circuits using basic logic gates
- Constructing complex systems from simple components
- Hardware verification of digital circuits

---

## 📂 Repository Contents
- Circuit diagrams
- Truth tables
- Calculations
- Hardware implementation images
- Lab documentation
