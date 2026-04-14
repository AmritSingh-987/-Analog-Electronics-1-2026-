Assignment 2.5 – Temperature Effects on Diode Behavior
(Amrit Singh)
Simulation Setup
The standard test circuit was utilized, consisting of a voltage source (V1) connected in series with a 1 kΩ resistor and the diode, which is then tied to ground. A DC sweep was executed from -2 V to +2 V. This exact sweep was tested at two specific temperatures:

25°C
75°C
Key Observations
1. Forward Voltage (Vf)
When operating at 75°C, the diode begins to conduct at a reduced forward voltage compared to room temperature (25°C). The rise in thermal energy boosts the diode's saturation current and overall carrier activity, meaning less voltage is required to achieve the same amount of current. Consequently, the entire "turn-on" curve shifts to the left (resulting in a lower Vf) as the temperature increases.

2. Reverse Leakage Current
The reverse leakage current is significantly higher at 75°C than at 25°C. This occurs because the elevated temperature generates a larger number of minority carriers within the PN junction, leading directly to increased leakage when the component is reverse-biased.

Practical Implications in Real Systems
Fluctuations in temperature directly impact the performance of real-world components like rectifiers, clamping circuits, and protection diodes:

A reduced forward voltage (Vf) at elevated temperatures alters expected output voltage levels (for instance, causing slight variations in a power supply's DC output).
Increased leakage current in hot conditions can lead to unwanted standby power consumption, measurement inaccuracies, or unintended bias shifts within highly sensitive electronic circuits.
