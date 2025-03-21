# Arduino Nano 4×4×4 LED Cube Display

## 📌 Introduction
This project is a **4×4×4 LED Cube Display** controlled by an **Arduino Nano**. The cube can display simple patterns, animations, or even react to input signals. This repository contains the necessary code, circuit diagram, and setup instructions to build and customize your own LED cube project.

---

## 🔥 Features
- **Compact Design** – Uses an **Arduino Nano** for space-efficient control.
- **Customizable Patterns** – Modify the code to create different LED animations.
- **Low Power Consumption** – Optimized for minimal energy usage.
- **Beginner-Friendly** – Easy to assemble and program.
- **Modular Code** – Easily extendable for more complex designs.

---

## 📦 Components Required
| Component               |   Quantity     |
|-------------------------|----------------|
|       Arduino Nano / Arduino UNO      | 1              |
|       4×4×4 LED Cube    | 64 LED lights  |
|       Resistors (1.2kΩ) | 4 in each layer|
|       Jumper Wires      | As needed      |
|       Breadboard / Vero Board /  PCB     | 1              |
|       Power Supply (5V) | 1              |
|       Solder machine  , flux & soldering wire         | 1              |
|       Container (optional) | 1              |
-------

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

## 📜 Installation & Usage

### 1️⃣ Clone the Repository
```bash
  git clone https://github.com/W-N-R/arduino-led-cube.git
```

### 2️⃣ Install Arduino IDE & Required Libraries
- Download and install **Arduino IDE** from [here](https://www.arduino.cc/en/software).
- Install any required libraries (if applicable).

### 3️⃣ Upload the Code
1. Open **Arduino IDE**.
2. Load the `.ino` file from the **/code** folder.
3. Select **Arduino Nano** as the board.
4. Choose the correct **COM port**.
5. Click **Upload**.

### 4️⃣ Test & Modify
- Once uploaded, observe the **LED cube animations**.
- Modify the code to create **custom patterns**!

---

## 🎯 How It Works
- The **Arduino Nano** controls the **4×4×4 LED cube** by rapidly switching LEDs on/off in layers.
- The program defines **patterns** in an array and updates the display accordingly.
- **Multiplexing** is used to control all 64 LEDs with fewer pins.
- You can create custom **animations** by modifying the pattern arrays.

---

## 🛠️ Customization
Want to add new patterns?
- Edit the **array values** inside the code.
- Adjust the **timing** for smooth animations.
- Experiment with **different LED configurations**.

---

## 💡 Troubleshooting
❌ **LEDs not lighting up?**
   - Check wiring connections.
   - Ensure **Arduino Nano** is correctly powered.

❌ **Wrong pattern displayed?**
   - Verify **row/column/layer mapping** in the code.
   - Try swapping LED connections.

❌ **Arduino not detected?**
   - Check USB connection.
   - Install correct **drivers** for Arduino Nano.

---

## 🤝 Contributions
Feel free to **contribute** by:
- Adding new animations.
- Improving circuit design.
- Optimizing code for efficiency.

To contribute, **fork the repository**, make changes, and submit a **pull request**! 🚀

---

## 📜 License
This project is open-source under the **MIT License**. You are free to use, modify, and distribute it.

---

## 📞 Contact
For any questions or suggestions, feel free to **open an issue** on GitHub.

Happy Coding! 🎯🚀

