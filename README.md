# Computer Organization Experiment

计算机组成原理实验

[TOC]

> Last Revised: `5/22/2017`

## Project 1

[Jump to directory](Project_1/)

单周期处理器开发

#### Instruction Set

> Total: 12

| Status 	| Ins Type 	| op 		| func 	| ALUctr 	| Branch	| Jump	| RegDst	| ALUSrc	| MemtoReg	| RegWr	| MemWr	| ExtOp	|
|:-------: 	|:--------:	|:------:	|:------:	|:------:	|:----: 	|:----: 	|:----: 	|:----: 	|:----: 	|:----: 	|:----: 	|:----: 	|
|`no tested`	| addu 	| 000000 	| 100000 	| 0000 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| add 	| 000000 	| 100000 	| 0001 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| subu 	| 000000 	| 100010 	| 1000 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| sub 	| 000000 	| 100010 	| 1001 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| and 	| 000000 	| 100100 	| 0010 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| or 	| 000000 	| 100101 	| 0011 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| sltu 	| 000000 	| 101010 	| 1010 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| slt 	| 000000 	| 101010 	| 1011 	| 0 	| 0 	| 1 	| 0 	| 0 	| 1 	| 0 	| x 	|
|`no tested`	| beq 	| 000100 	| x 	| 1001 	| 1 	| 0 	| x 	| 0 	| x 	| 0 	| 0 	| x 	|
|`no tested`	| jump 	| 000010 	| x 	| x 	| 0 	| 1 	| x 	| x 	| x 	| 0 	| 0 	| x 	|
|`no tested`	| lw 	| 100011 	| x 	| 0001 	| 0 	| 0 	| 0 	| 1 	| 1 	| 1 	| 0 	| 1 	|
|`no tested`	| sw 	| 101011 	| x 	| 0001 	| 0 	| 0 	| x 	| 1 	| x 	| 0 	| 1 	| 1 	|


### Datapath Module

- [x] [PC (Program Counter)](Project_1/datapath/pc.v)
- [x] [NPC (Next PC)](Project_1/datapath/npc.v)
- [x] [RF (Register File)](Project_1/datapath/rf.v)
- [x] [ALU (Arithmetic Logic Unit)](Project_1/datapath/alu.v)
- [x] [EXT (Extended Unit)](Project_1/datapath/ext.v)
- [x] [IM (Instruction Memory)](Project_1/datapath/im.v) `4KB (32bits*1024)`
- [x] [DM (Data Memeory)](Project_1/datapath/dm.v) `4KB(32bits*1024)`

### Control Module

- [x] [CTRL (Controller)](Project_1/control/ctrl.v)

### Creator

- [x] [MIPS (Creater)](Project_1/mips.v)
