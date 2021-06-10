## Build your model

Now that you have an idea, it's time to build your model. Below are a few tips that might help you to produce the model you want.

--- collapse ---
---
title: Using a craft or utility knife
---

Craft and utility knives are very useful when making models, but you must be very careful when using them, as they are extremely sharp and can easily cause an injury. If you are using a craft or utility knife, make sure you have a responsible adult with you, or ask them to do the cutting for you if you prefer. It's also a good idea to use a cutting mat to protect the surface you are working on. If you don't have a cutting board, a kitchen chopping board is a great alternative.

![A box cutting knife.](https://upload.wikimedia.org/wikipedia/commons/c/cf/Box-cutter.jpg)

--- /collapse ---

--- collapse ---
---
title: Joining together jumper wires
---

You might need extra-long wires to attach your LED to your Raspberry Pi pins. You can do this by 'daisy chaining' wires together. For instance, to make an extra-long F-F wire, you can attach an M-F wire to an F-F wire.

![An M-F wire attached to an F-F wire.](images/daisy-chain.jpg)

The problem with this method is that often the wires will become detached from each other. You can use a small piece of tape to secure the connection.

![An M-F wire taped to an F-F wire.](images/tape-daisy-chain.jpg)

--- /collapse ---

--- collapse ---
---
title: Short circuits
---

As the legs of the LEDs are often exposed, it is easy for to create a **short circuit** if the exposed legs touch each other. This will stop your LED from working. A little bit of tape wrapped around each LED leg will prevent this.

![An LED attached to jumper wires with tape insulating each LED leg.](images/insulated-led.jpg)

This will also help to keep the LED attached to its jumper wires.

--- /collapse ---

--- collapse ---
---
title: Multiple LEDs
---

You might have only used a single LED in your projects before, but you can use lots of LEDs if you want to. Each LED will need its long leg attached to a numbered pin and the short leg attached to a ground pin. You can see the location of all the numbered pins and ground pins in the diagram below.

![Raspberry Pi pinout.](https://www.raspberrypi.org/documentation/usage/gpio/images/GPIO-Pinout-Diagram-2.png)

To control the LEDs, you just change the pin number in your Scratch program so it corresponds to the pin the LED is attached to.

```blocks3
turn LED (21 v) [on v] ::extension
turn LED (26 v) [off v] ::extension
```

--- /collapse ---
