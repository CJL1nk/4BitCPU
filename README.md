instruction format

```
weoo oooo ddss aaaa aaaa
0000 0000 0000 0000 0000

w - Write
e - Enable immediate
o - operation
d - dest register
s - source register
a - immediate val/address
```

Current operations:
* add (00)
* sub (01)
* mul (10)
* div (11)

Any of these operations can operate on an immediate value by flipping the E bit high.

For the registers to update accordingly, the Write bit must be flipped high. This makes an instruction 0000000000000000 effectively a noop.
