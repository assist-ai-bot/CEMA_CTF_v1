# Task 8 — Gimbal program

`gimbal.vm` is a raw instruction stream. Each instruction is three bytes. The flag is the console output as text.

Submit it in this shape and no other. The text below is an example of the characters, not the program:

```
Intern_Pro_Max{lamp-3}
```

Lowercase letters, one hyphen, then one digit. No spaces.

Opcode `0x0B` behaves as follows:

| `rA` before | operand B | `rA` after |
| --- | --- | --- |
| `0x03` | 2 | `0x0C` |
| `0x81` | 1 | `0x03` |
