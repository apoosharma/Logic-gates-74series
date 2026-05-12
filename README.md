# Logic Gates using 74-Series ICs 🔌

Hands-on implementation and verification of basic logic gates 
using 74-series TTL ICs on a breadboard.

---

## 🧰 Components Used

| Component | Function |
|-----------|---------|
| SN74LS08N | AND Gate |
| SN74HC32N | OR Gate |
| SN74LS00N | NAND Gate |
| SN74HC04N | NOT Gate (Hex Inverter) |
| DIP Switch | Logic Input (A & B) |
| LED + 1kΩ | Output Indicator |
| 10kΩ resistors | Pull-up resistors |
| Breadboard Power Module | 5V Supply |

---

## ⚙️ How It Works

Each IC is powered at 5V (Pin 14 = VCC, Pin 7 = GND).  
DIP switches act as logic inputs with 10kΩ pull-up resistors.  
LED with 1kΩ series resistor shows the output visually.

---

## 📊 Truth Tables & Results

### AND Gate (SN74LS08N)
| Input A | Input B | Output |
|---------|---------|--------|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 ✅ |

### OR Gate (SN74HC32N)
| Input A | Input B | Output |
|---------|---------|--------|
| 0 | 0 | 0 |
| 0 | 1 | 1 ✅ |
| 1 | 0 | 1 ✅ |
| 1 | 1 | 1 ✅ |

### NAND Gate (SN74LS00N)
| Input A | Input B | Output |
|---------|---------|--------|
| 0 | 0 | 1 ✅ |
| 0 | 1 | 1 ✅ |
| 1 | 0 | 1 ✅ |
| 1 | 1 | 0 |

### NOT Gate (SN74HC04N)
| Input A | Output |
|---------|--------|
| 0 | 1 ✅ |
| 1 | 0 |

---

## 🔍 Key Observations

- Pull-up resistors are essential — floating inputs cause random output
- 5V supply is critical — 9V damages 74xx series ICs
- LED polarity matters — longer leg faces the resistor
- All unused IC inputs must be tied to VCC or GND

---

## 📚 What I Learned

- How TTL logic ICs work internally
- Practical difference between AND/NAND/OR/NOT behavior
- Breadboard circuit debugging techniques
- Importance of proper power supply for digital ICs

---

## 🔗 References

- [SN74LS08N Datasheet](https://www.ti.com/product/SN74LS08)
- [SN74HC32N Datasheet](https://www.ti.com/product/SN74HC32)

---
⭐ Star this repo if it helped you!
