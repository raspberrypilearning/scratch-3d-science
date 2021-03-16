## Build your model

Now that you have an idea, it is time to build your model. Below are a few tips that might help you to produce the model you want.

--- collapse ---
---
title: Using a craft or utility knife
---

Craft and utility knives are very useful when making models, but you must be very careful when using them, as they are extremely sharp and can easily cause an injury. If you are using a craft or utility knife, make sure you have a responsible adult with you, or if you are not confident, ask them to do the cutting for you. It's also a good idea to use a cutting mat, to protect the surface you are working on, but a kitchen chopping board is a great alternative.

![a box cutting knife](https://upload.wikimedia.org/wikipedia/commons/c/cf/Box-cutter.jpg)

--- /collapse ---

--- collapse ---
---
title: Joining together jumper leads.
---

You might need extra-long leads to attach your LED to your Raspberry Pi pins. You can do this by "daisy chaining" leads together. For instance, to make an extra-long F-F lead, you can use a single M-F lead with another F-F lead.

![an m to f lead attached to an f to m lead](images/daisy-chain.jpg)

The problem with this method is that often the leads will become detached from each other. It's often useful to use a small piece of tape to secure the connection.

![an m to f lead taped to an f to m lead](images/tape-daisy-chain.jpg)

--- /collapse ---

--- collapse ---
---
title: Short circuits
---

As the legs of the LEDs are often exposed, it is easy for them to touch each other, and create what is called a **short circuit**. This will stop your LED from working. A little bit of tape wrapped around each LED leg will prevent this from happening.

![an led attached to jumper leads with tape insulating each led leg](images/insulated-led.jpg)

This will also help to keep the LED attached to it's jumper leads.

--- /collapse ---

--- collapse ---
---
title: Multiple LEDs
---

Up until now, you might have only used a single LED in your projects. There's no reason that you can't use many more LEDs though. Each LED will need to use a numbered pin attached to the long leg and a Ground pin attached to the short leg. You can see the location of all the numbered pins and ground pins on the diagram below.

![raspberry pi pinout](https://www.raspberrypi.org/documentation/usage/gpio/images/GPIO-Pinout-Diagram-2.png)

To control the LEDs, you just use the pin number in your Scratch program

```blocks3
turn LED (21 v) [on v] ::extension
turn LED (26 v) [off v] ::extension
```

--- /collapse ---