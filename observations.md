# Observations & Learnings 🔍

## Challenges Faced

- **9V battery damaged nothing but didn't work** — 74xx series strictly needs 5V
- **LED not lighting up** — forgot to connect negative rail, polarity matters
- **Random output flickering** — fixed by adding 10kΩ pull-up resistors on inputs
- **DIP switch confusion** — had to identify correct pin rows before wiring

---

## Gate-wise Observations

| Gate | IC Used | Observation |
|------|---------|-------------|
| AND | SN74LS08N | Output HIGH only when BOTH inputs HIGH |
| OR | SN74HC32N | Output HIGH when ANY input is HIGH |
| NAND | SN74LS00N | Opposite of AND — LOW only when both HIGH |
| NOT | SN74HC04N | Single input — always flips the signal |

---

## Key Learnings

- Pull-up resistors prevent floating inputs — critical for clean logic levels
- TTL ICs are very sensitive to supply voltage — always verify before powering
- Breadboard power supply modules are better than raw batteries for digital circuits
- Always connect unused IC inputs to VCC or GND — never leave them floating
- LED always needs a current limiting resistor — no resistor = instant burnout

---

## Real World Applications Understood

- AND gate → Safety systems (both conditions must be true)
- OR gate → Alarm systems (any trigger activates it)
- NOT gate → Signal inversion, enable/disable logic
- NAND gate → Universal gate, used in RAM and processor circuits
