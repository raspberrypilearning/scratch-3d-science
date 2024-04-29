\--- question ---

---

## 图例：问题2/3

以下哪块会让 LED 随机模式闪烁。

\--- choices ---

- ( ) 1:

```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (0.5) seconds
```

\--- feedback ---

不，该脚本会让你的 LED 定期闪烁 - 每 0.5 秒一次。

\--- /feedback ---

- (x) 2:

```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (pick random (0.1) to (0.5)) seconds
```

\--- feedback ---

是的，这个脚本会让你的 LED 随机闪烁。

\--- /feedback ---

- ( ) 3:

```blocks3
when flag clicked
toggle LED (21 v) ::extension
wait (pick random (0.1) to (0.5)) seconds
```

\--- feedback ---

不，这个脚本只会切换 LED 一次，而不是按照某种模式。

\--- /feedback ---

- ( ) 4:

```blocks3
when flag clicked
forever
toggle LED (pick random (1) to (10)) ::extension
wait (1) seconds
```

\--- feedback ---

不对. 这将使 LED 随机闪烁一秒

\--- /feedback ---

\--- /choices ---

\--- /question ---
