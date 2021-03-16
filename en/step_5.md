## Control your LEDs

Hopefully you've now built your model, with your LEDs all wired up to your Raspberry Pi. Make sure you remember which numbered pins you used, because now it is time to add some code to control your LEDs.

Have a look at the options below, for some different ideas on how the LEDs can be turned on and off.

--- collapse ---
---
title: Blink a regular pattern
---

The following blocks will create a regular blinking pattern on an LED. By changing the `wait`{:class='block3control'} time, you can make the LED blink faster or slower.

```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (1) seconds
```

--- /collapse ---

--- collapse ---
---
title: Random blinking
---

By using the `pick random`{:class='block3operators'} block, the blinking of and LED can appear to be completely random. Changing the values used in the `pick random`{:class='block3operators'} block will change how quickly the LED blinks.

```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait <pick random (0.1) to (0.5)> seconds
```

--- /collapse ---

--- collapse ---
---
title: Click a sprite to control an LED
---

By using the `when this sprite clicked`{:class='block3events'} block, the LED can be turned on for a few seconds.

```blocks3
when this sprite clicked
turn LED (21 v) [on v] ::extension
wait (2) seconds
turn LED (21 v) [off v] ::extension
```

--- /collapse ---

--- collapse ---
---
title: Press a key to control an LED
---

By using the `when key pressed`{:class='block3events'}, an LED can be turned on and off by using the keyboard attached to your Raspberry Pi.

```blocks3
when [up arrow v] key pressed
turn LED (21 v) [on v] ::extension

when [down arrow v] key pressed
turn LED (21 v) [off v] ::extension
```

--- /collapse ---

--- collapse ---
---
title: Using the Sensing menu to control an LED
---

The `sensing`{:class='block3sensing'} menu has blocks that can detect events that happen in Scratch and you can use these to trigger your LEDs. Here's an example using the mouse pointer. When a sprite is touched by the mouse pointer, the LED will come on, and then turn off when the pointer moves away.\

```blocks3
when flag clicked
forever
if <touching (mouse-pointer v)?> then
turn LED (21 v) [on v] ::extension
else
turn LED (21 v) [off v] ::extension
```



--- /collapse ---