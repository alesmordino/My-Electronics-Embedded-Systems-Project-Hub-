## 🔌 Circuit Diagram ASCII
Refer to the **/circuit_diagrams** folder for detailed schematics.

### Basic Wiring:
- Connect **Arduino Nano digital pins** to LED cube row/column/layer pins.
- Use **resistors** (1.2kΩ for layers) to limit current.
- Ensure **correct power supply connections** to avoid damage.
- If using a **Vero board or PCB**, ensure proper soldering and layout to minimize short circuits.
<  +5V  
   │  
  [1.2kΩ]─┬── Layer 1  
  [1.2kΩ]─┬── Layer 2  
  [1.2kΩ]─┬── Layer 3  
  [1.2kΩ]─┬── Layer 4  
   │  
  GND  
   
   Columns (via 330Ω resistors)  
   │   │   │   │  
  ●──●──●──●  → Arduino Pins  
  ●──●──●──●  
  ●──●──●──●  
  ●──●──●──●  
   
  4×4 LEDs per layer, controlled via multiplexing  
>

---
