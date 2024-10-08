# Digital And Number Systems

## 1. Digital Systems Overview

- A **digital system** processes discrete information inputs, internal information (system state), and generates discrete outputs.
  
  - **System State**: Information retained by the system at any given time.
  - **Control Unit**: Manages the flow of information within the system.
  - **Datapath**: Performs arithmetic and other data processing operations.
  - **CPU**: Combination of the datapath and control unit.

---

## 2. Abstraction Layers in Computer Systems

- **Abstraction**: Modern computer systems are built using layers of abstraction. Each layer hides the complexity of the one below it.

---

## 3. Signals in Digital Systems

- **Signal**: An information variable represented by physical quantities.
  - **Digital Signal**: Discrete values like binary values (0 and 1).
  - **Binary Values**: 
    - Can be represented as:
      - 0 and 1
      - True (T) and False (F)
      - High (H) and Low (L)
      - On and Off

---

## 4. Analog vs Digital Signals

- **Analog Systems**: Signals vary continuously over a range.
- **Digital Systems**: Signals assume only discrete values, which allows for greater accuracy.

---

## 5. Key Historical Developments

- **Charles Babbage**: Designed the first mechanical computer in the 1830s but never built it. The first complete Babbage Engine was constructed in 2002.
- **ENIAC**: The first programmable general-purpose electronic digital computer, built in 1946.

---

## 6. Moore’s Law

- **Moore's Law**: The number of transistors in a dense integrated circuit (IC) doubles about every two years, leading to increased computational power.

---

## 7. Binary Digits and Logic Levels

- **Bit**: A binary digit, either 0 or 1.
  - In circuits, binary digits are represented by different voltage levels.
  - **Logic Levels**: The voltage values that represent 1 (HIGH) and 0 (LOW).
  - Common logic level ranges in digital circuits (e.g., CMOS technology):
    - **High**: 2V to 3.3V
    - **Low**: 0V to 0.8V

---

## 8. Digital Waveforms

- A **digital waveform** consists of voltage levels transitioning between HIGH and LOW states.
- **Pulse**: A change from LOW to HIGH and back to LOW (positive-going pulse), or from HIGH to LOW and back to HIGH (negative-going pulse).

### Waveform Characteristics:
- **Periodic Waveform**: Repeats at regular intervals, with a specific period (T).
- **Frequency (f)**: The rate at which the waveform repeats, measured in Hertz (Hz).
  - Frequency and period are related by \( f = \frac{1}{T} \).
- **Duty Cycle**: The ratio of the pulse width (\(t_W\)) to the period (\(T\)).

---

## 9. Timing and Data Transfer

- **Clock**: A timing waveform used to synchronize operations in digital systems.
  - Each change in level (rising or falling edge) of the clock waveform is crucial for timing circuit behavior.
  
- **Timing Diagrams**: Graphical representations of digital signals over time, showing the timing relationships between different signals.

- **Data Transfer**:
  - **Serial Transfer**: Bits are transmitted one at a time over a single channel.
  - **Parallel Transfer**: Multiple bits are transmitted simultaneously over multiple channels.

---

## 10. Number Systems

- **Decimal System**: Base-10 system, used in everyday calculations.
- **Binary System**: Base-2 system, used in digital systems.
  - **MSB (Most Significant Bit)**: The leftmost bit.
  - **LSB (Least Significant Bit)**: The rightmost bit.

### Binary Number Range:
- With **N** bits, numbers can range from 0 to \(2^N - 1\).
  - Example: 8 bits range from 0 to 255.

### Binary to Decimal Conversion:
- Convert binary numbers to decimal by summing powers of 2 for each bit position.

### Decimal to Binary Conversion:
- Convert a decimal number to binary by repeatedly dividing by 2 and recording remainders.

---

## 11. Octal and Hexadecimal Systems

- **Octal System**: Base-8, groups of 3 binary digits.
- **Hexadecimal System**: Base-16, groups of 4 binary digits.
  - Easier for humans to read and write compared to long binary numbers.

### Conversion:
- Convert binary to octal/hex by grouping binary digits and converting each group to its octal or hexadecimal equivalent.

---

## 12. Complements of Binary Numbers

- **1's Complement**: Invert all bits (0 → 1 and 1 → 0).
- **2's Complement**: Add 1 to the 1's complement. Used for representing negative numbers.

### Signed Numbers:
- **Sign-Magnitude Representation**: Leftmost bit indicates the sign (0 for positive, 1 for negative).
- **2's Complement Representation**: Common method for representing signed numbers in digital systems.

---

## 13. Arithmetic Operations with Signed Numbers

- **Addition**: Add normally and discard any carry bits.
- **Subtraction**: Convert the subtrahend to its 2's complement and add.
- **Multiplication**: Performed using multiple additions.

### Overflow:
- Occurs when the result of an operation exceeds the range of the number representation.

---

## 14. Binary Coded Decimal (BCD)

- **BCD**: A binary encoding of decimal numbers where each decimal digit is represented by a group of 4 bits.
  - Example: Decimal 35 → BCD 0011 0101.
  
- Commonly used in systems where binary data must be displayed or entered in decimal form (e.g., calculators, digital displays).

---

## 15. Gray Code

- **Gray Code**: A binary numeral system where two successive values differ by only one bit.
  - Used in error correction in digital communications and for minimizing errors in analog to digital conversion (e.g., shaft position encoders).

### Conversion:
- **Binary to Gray**: The MSB is the same, and each subsequent bit is XORed with the previous binary bit.
- **Gray to Binary**: Reverse the process, starting with the MSB.

---

## 16. ASCII and Alphanumeric Codes

- **ASCII (American Standard Code for Information Interchange)**: A 7-bit code representing letters, numbers, and control characters.
  - **Extended ASCII**: An 8-bit code used to represent additional symbols and characters (e.g., foreign alphabets, mathematical symbols).
  
- **Unicode**: A global standard for encoding characters from most world languages.

---

## 17. Error Detection

- **Parity Bit**: A single bit added to a binary string to make the number of 1s either even or odd.
  - **Even Parity**: The number of 1s in the data plus the parity bit is even.
  - **Odd Parity**: The number of 1s in the data plus the parity bit is odd.
  - Parity bits are commonly used for simple error detection in communication systems.

---
