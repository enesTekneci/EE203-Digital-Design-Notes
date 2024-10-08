# EE203 Digital Design Study Notes

## 2. Logic Gates

### Instructor: Dr. Abdulkadir Köse  
**FALL 2024**

---

## 1. Inverter (NOT Gate)

- **Inversion (complementation)**: Changes 1 to 0 and 0 to 1.
- Also called a **NOT gate**.
  
### Boolean Expression:
- Output = `A'` (also written as `NOT A` or `A̅`)

### Application:
- **1's complement** of a binary number, used in binary arithmetic.

| Input | Output |
|-------|--------|
|   0   |    1   |
|   1   |    0   |

---

## 2. AND Gate

- **AND Gate**: Produces an output of 1 only when **all inputs** are 1.
- Multiple inputs, single output.

### Boolean Expression:
- For two inputs: `X = A • B` or `X = AB`
  
### Application Example: **Masking**
- Used to **clear specific bits** in a number.
  - Example: Clear the right four bits.
  - Mask: `11110000`
  - Input: `10100101`
  - Result of `Mask AND Input` → `10100000`

| Input A | Input B | Output |
|---------|---------|--------|
|    0    |    0    |    0   |
|    0    |    1    |    0   |
|    1    |    0    |    0   |
|    1    |    1    |    1   |

### Real-Life Example: **Seatbelt Alarm Circuit**
- The alarm will sound if the seatbelt is unbuckled while the ignition switch is on for 30 seconds.

---

## 3. OR Gate

- **OR Gate**: Produces an output of 1 if **any input** is 1.
- Multiple inputs, single output.

### Boolean Expression:
- For two inputs: `X = A + B`

### Application Example: **Masking**
- Used to **set specific bits** in a number.
  - Example: Set the right four bits.
  - Mask: `00001111`
  - Input: `10100101`
  - Result of `Mask OR Input` → `10101111`

| Input A | Input B | Output |
|---------|---------|--------|
|    0    |    0    |    0   |
|    0    |    1    |    1   |
|    1    |    0    |    1   |
|    1    |    1    |    1   |

### Real-Life Example: **Intrusion Detection System**
- The alarm activates if any door or window is open in a room.

---

## 4. NAND Gate

- **NAND Gate**: Produces an output of 0 only when **all inputs** are 1.
- **Universal Gate**: All other gates (AND, OR, NOT, NOR) can be implemented using NAND gates.

### Boolean Expression:
- For two inputs: `X = (AB)'` or `X = A NAND B`

| Input A | Input B | Output |
|---------|---------|--------|
|    0    |    0    |    1   |
|    0    |    1    |    1   |
|    1    |    0    |    1   |
|    1    |    1    |    0   |

### Real-Life Example: **Tank Level Indicator System**
- If both tanks have more than 25% liquid, a green LED will light up using a NAND gate.

---

## 5. NOR Gate

- **NOR Gate**: Produces an output of 1 only when **all inputs** are 0.
- **Universal Gate**: All other gates (AND, OR, NOT, NAND) can be implemented using NOR gates.

### Boolean Expression:
- For two inputs: `X = (A + B)'` or `X = A NOR B`

| Input A | Input B | Output |
|---------|---------|--------|
|    0    |    0    |    1   |
|    0    |    1    |    0   |
|    1    |    0    |    0   |
|    1    |    1    |    0   |

### Real-Life Example: **Landing Gear Indicator System**
- A green LED turns on when all landing gears are extended using a NOR gate.

---

## 6. XOR Gate (Exclusive OR)

- **XOR Gate**: Produces an output of 1 only when the inputs are different.
- Used in **half-adders** and **parity generators**.

### Boolean Expression:
- For two inputs: `X = A ⊕ B = A'B + AB'`

| Input A | Input B | Output |
|---------|---------|--------|
|    0    |    0    |    0   |
|    0    |    1    |    1   |
|    1    |    0    |    1   |
|    1    |    1    |    0   |

---

## 7. XNOR Gate (Exclusive NOR)

- **XNOR Gate**: Produces an output of 1 only when the inputs are the same.
- Sometimes called the **equivalence gate**.

### Boolean Expression:
- For two inputs: `X = A ⊕ B' = A'B' + AB`

| Input A | Input B | Output |
|---------|---------|--------|
|    0    |    0    |    1   |
|    0    |    1    |    0   |
|    1    |    0    |    0   |
|    1    |    1    |    1   |

---

## Exercises

### XOR Application: Lamp Control Circuit
- A lamp is on (high) when an odd number of switches (A, B, C) are on.
- The logic expression for the lamp is:
  - `L = A ⊕ B ⊕ C`

---

## Timing Diagrams
- Timing diagrams are graphical representations that show how inputs and outputs of a digital system change over time.
- Useful in understanding the relationship between multiple signals in logic circuits.

---

## Conclusion
This section provided a foundation on various logic gates, their Boolean expressions, and real-world applications. Understanding these gates is crucial for designing and analyzing more complex digital circuits.
