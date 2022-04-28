

--- question ---

---
legend: Question 2 of 3
---

Which of the following blocks would make an LED blink in a random pattern.

--- choices ---

- ( ) 1: 
```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (0.5) seconds
```

--- feedback ---

No, this script will make your LED blink regularly - every 0.5 seconds.

--- /feedback ---

- (x) 2: 
```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (pick random (0.1) to (0.5)) seconds
```

--- feedback ---

Yes, this script will make your LED blink in a random pattern.

--- /feedback ---

- ( ) 3: 
```blocks3
when flag clicked
toggle LED (21 v) ::extension
wait (pick random (0.1) to (0.5)) seconds
```

--- feedback ---

No, this script will only toggle the LED once, rather than in a a pattern

--- /feedback ---

- ( ) 4: 
```blocks3
when flag clicked
forever
toggle LED (pick random (1) to (10)) ::extension
wait (1) seconds
```

--- feedback ---

No. This would make a random LEDs blink for one second

--- /feedback ---

--- /choices ---

--- /question ---