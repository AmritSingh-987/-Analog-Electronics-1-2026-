# Assignment 1.2: Simple Resistive Voltage Divider
**Course:** Analog Electronics 1 (IT24SP)
**Student:** Amrit SIngh

## Description
This project demonstrates the behavior of a simple resistive voltage divider circuit simulated in LTspice. The goal is to observe how voltage is distributed across resistors in series and verify the results against theoretical calculations.

## Circuit Specifications
- **Input Voltage (V1):** 10V DC
- **Resistor 1 (R1):** 1kΩ
- **Resistor 2 (R2):** 1kΩ
- **Simulation Type:** Transient Analysis (.tran 100ms)

## Theoretical Calculations
According to the Voltage Divider Rule:

Vout = Vin* R2/(R1+R2)
Vout = 10* 1000/(1000+1000) = 5V


The total current in the circuit is:
$I = \frac{V_{in}}{R_{total}} = \frac{10V}{2k\Omega} = 5mA$

## Simulation Results
The simulation confirms the theory:
- **Measured Output Voltage:** 5V
- **Measured Current:** 5mA (Magnitude)

### Circuit Schematic
.asc file

### Output of LTspice
Voltage divider circuit.jpg

