## 控制您的 LED

现在您应该已经构建了模型并将 LED 连接到了 Raspberry Pi。 确保您记住使用了哪些编号的引脚，因为现在是时候添加一些代码来控制您的 LED 了。

请查看以下选项，了解有关如何打开和关闭 LED 的一些不同创意。

--- collapse ---
---
title: 常规闪烁模式
---

以下代码块将为 LED 创建规则的闪烁模式。 通过改变`wait`{:class='block3control'}时间，您可以使LED闪烁得更快或更慢。

```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (1) seconds
```

--- /collapse ---

--- collapse ---
---
title: 随机闪烁
---

通过使用`随机选择`{class='block3operators'} 块，LED 的闪烁看起来是完全随机的。 改变`随机选择`{:class='block3operators'} 块中使用的值将会改变 LED 闪烁的速度。

```blocks3
when flag clicked
forever
toggle LED (21 v) ::extension
wait (pick random (0.1) to (0.5)) seconds
```

--- /collapse ---

--- collapse ---
---
title: 单击精灵来控制 LED
---

使用 `当这个精灵单击`{:class='block3events'} 块时，LED 可以开启几秒钟。

```blocks3
when this sprite clicked
turn LED (21 v) [on v] ::extension
wait (2) seconds
turn LED (21 v) [off v] ::extension
```

--- /collapse ---

--- collapse ---
---
title: 点击按键来控制 LED
---

通过使用`按下按键时`{:class='block3events'} 块，可以使用连接到树莓派的键盘来打开和关闭 LED。

```blocks3
when [up arrow v] key pressed
turn LED (21 v) [on v] ::extension

when [down arrow v] key pressed
turn LED (21 v) [off v] ::extension
```

--- /collapse ---

--- collapse ---
---
title: 使用感应菜单控制 LED
---

`sensing`{:class='block3sensing'} 菜单具有可以检测 Scratch 中发生的事件的块，您可以使用这些块来触发 LED。 这是使用鼠标指针的示例。 当鼠标指针触碰精灵时，LED 会亮起，而当指针移开时，LED 会熄灭。

```blocks3
when flag clicked
forever
if <touching (mouse-pointer v) ?> then
turn LED (21 v) [on v] ::extension
else
turn LED (21 v) [off v] ::extension
```

--- /collapse ---
