--- question ---

---
legend: Question 2 of 3
---

Look at the following circuit used to test if an LED is working. The LED does not light up. What is the most likely reason the LED is not working
![an LED and resistor connected to a Raspberry Pi. The long leg of the LED is connected to the resistor, which is connected to a ground pin. The short leg of the LED is connected to a 3V3 pin](images/led-wiring.png)

--- choices ---

- ( ) 1: The wrong colour wires have been used to connect the LED to the Raspberry Pi

--- feedback ---

No. Wires all work the same way, no matter what their colour. It's just helpful to use certain colours for certain jobs, to make it easier to debug your circuits.

--- /feedback ---

- (x) 2: The LED has been connected the wrong way around.

--- feedback ---

Excellent. The long leg of the LED should connect to a 3V3 pin and the short leg to a ground pin

--- /feedback ---

- ( ) 3: The resistor should be the other side of the LED

--- feedback ---

No. Resistors will protect an LED whether they are connected to the short leg or the long leg.

--- /feedback ---

- ( ) 4: Pin 21 should have been used

--- feedback ---

No. Pin 21 is a programable pin, which is often used to control an LED. You use a 3V3 pin to test whether an LED is working.

--- /feedback ---

--- /choices ---

--- /question ---