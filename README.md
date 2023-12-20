## ep. 1

```javascript
const memory = createMemory(256); // create memory as bits
const writableBytes = new Uint8Array(memory.buffer);

const cpu = new CPU(memory); // create an CPU object

writableBytes[0] = instructions.MOV_LIT_R1; //
writableBytes[1] = 0x12; // 0x1234
writableBytes[2] = 0x34;

cpu.step(); // read the first line than increase the index of array, then fetch the next 2 line
// and increment the index by 2
```

## ep. 3

implementing stack to be able to have subroutines . push literals/registers and pop them, return from stack
