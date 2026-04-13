# Assignment 3.2: Full-Wave Rectifier Simulation (LTspice)
**Student Name:** Amrit Singh

## 1. Simulation Setup
* **Circuit Type:** Full-wave Bridge Rectifier
* **Input Voltage ($V_1$):** AC Sine Wave
    * **Peak Amplitude:** 100V
    * **Frequency:** 50Hz
* **Simulation Parameters:**
    * **Type:** Transient Analysis (`.tran`)
    * **Stop Time:** 40ms (Calculated to capture exactly two full cycles of a 50Hz signal)
    * **Time Step:** Automatic (optimized for waveform resolution)

## 2. Behavioral Analysis
The simulation results demonstrate **full-wave rectification**. 

### Observations:
* **Input Waveform:** The green trace `V(In+, In-)` shows a complete sinusoidal AC wave oscillating between $+100\text{V}$ and $-100\text{V}$.
* **Output Waveform:** The red trace `V(Vout)` shows that the negative half-cycles of the AC input have been "flipped" into the positive domain. This results in a pulsating DC output where the frequency is effectively doubled to $100\text{Hz}$.
* **Voltage Amplitude:** Because the circuit utilizes a resistor bridge ($R_1, R_2, R_3$ all at $2.2\text{k}\Omega$), the output peak is approximately $50\text{V}$. This occurs because the load resistor and the bridge resistors form a voltage divider: 
$$V_{peak\_out} \approx V_{peak\_in} \cdot \left(\frac{R_{load}}{R_{bridge} + R_{load}}\right)$$
* **Diode Function:** Diodes $D_1$ and $D_2$ act as one-way valves, ensuring that current always flows through the load resistor $R_3$ in the same direction, regardless of the AC input polarity.

## 3. Files in this Repository
 The LTspice schematic file.
 Screenshot of the circuit design.
 Screenshot showing the input sine wave vs. the rectified output.
