# arm-assembly-bcd-operations
ARM assembly programs for ASCII-BCD conversions and iterative subtraction using Keil uVision. Includes memory, register, and flag analysis.
# 🔧 ARM Assembly – BCD & ASCII Operations (Keil uVision)

This project includes ARM assembly implementations for number system conversions and arithmetic operations using Keil uVision.

---

## 📌 Tasks Implemented

### 🔹 1. ASCII → BCD Conversion

Convert the numbers **24, 35, 06** into:

* Unpacked BCD
* Packed BCD

Results are stored starting at:

```
0x20001000 (incremented by 4 bytes)
```

---

### 🔹 2. BCD → ASCII Conversion

Convert packed BCD values:

```
0x24, 0x35, 0x06
```

to ASCII format.

Stored at:

```
0x20002000
```

---

### 🔹 3. Iterative Subtraction (Branching)

Subtract the series:

```
1, 2, 3, ..., 50
```

from initial value:

```
1500
```

Stored at:

```
0x20003000
```

---

## ⚙️ Implementation Details

* ARM Assembly (Keil uVision)
* Use of registers R0–R5
* Memory addressing with post-increment
* Looping with `CMP` and `BNE`
* Bitwise operations (`AND`, `ORR`, `LSL`, `LSR`)

---

## 🧠 Key Concepts

* Packed vs Unpacked BCD
* ASCII encoding (0x30 offset)
* Loop control with branching
* Memory manipulation in ARM

---

## 📊 Results

### 🔹 Memory Outputs

* Unpacked BCD stored correctly (lower nibble extraction)
* Packed BCD formed using shift + OR
* ASCII conversion verified using `+0x30`
* Iterative subtraction stored step-by-step

👉 Assignment description confirms memory locations and operations 

---

## 🖼️ Simulation Evidence

Screenshots include:

* Register values
* Memory content changes
* Loop execution
* Flag status

---

## 📂 Files

* `ascii_to_bcd.s`
* `bcd_to_ascii.s`
* `subtract_series.s`
* Screenshots (results)

---

## 👨‍💻 Author

Murat Emre Demirci
Electrical & Electronics Engineering

---
