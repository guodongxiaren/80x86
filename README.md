# 80x86
x86汇编语言简要。包括Intel语法和AT&T语法
---------
>本目录依据是**Intel**语法，在指令具体介绍中有对应**AT&T**语法介绍

80x86指令系统可分为以下6组：
- 数据传送指令
- 算数指令
- 逻辑指令
- 串处理指令
- 控制转移指令
- 处理机控制指令

##数据传送指令
###通用数据传送指令
|指令|英文释义|说明
|:---:|-----|-----
|MOV|move|传送
|MOVSX|move with sign-extend|带符号扩展传送
|MOVZX|move with zero-extend|带零扩展传送
|PUSH|push onto the stack|进栈
|POP|pop from the stack|出栈
|XCHG|exchange|交换

###地址传送指令
|指令|英文释义|说明
|:---:|-----|-----
|LEA|load effective address|有效地址传送寄存器
|LDS|load DS with pointer|指针送寄存器和DS
|LES|load ES with pointer|指针送寄存器和ES
|LSS|load SS with pointer|指针送寄存器和SS

##算数指令
|加法指令|说明
|---|----
|ADD|加法
|ADC|带进位加法
|INC|加1
|XADD|交换并相加

|减法指令|说明
|---|----
|SUB|减法
|SBB|带借位减法
|DEC|减1
|NEG|求补
|CMP|比较
|`CMPXCHG`|比较并交换
|`CMPXCHG8B`|比较并交换8字节

|乘法指令|说明
|---|----
|MUL|无符号乘法
|IMUL|带符号乘法

|除法指令|说明
|---|----
|DIV|无符号除法
|IDIV|带符号除法

##逻辑指令
###逻辑运算指令
|指令|说明
|---|---
|AND|与
|OR|或
|NOT|非
|XOR|异或
|*TEST*|测试
|
###移位指令
|左移|说明|右移|说明
|-----|----|----|---
|SHAL|逻辑左移|SHR|逻辑右移
|SAL|算数左移|SAR|算数右移
|ROL|循环左移|ROR|循环右移
|RCL|带进位循环左移|RCR|带进位循环右移
|SHLD|双精度左移|双精度右移