# 80x86
x86汇编语言简要。包括Intel语法和AT&T语法
---------
80x86指令系统可分为以下6组：
- 数据传送指令
- 串处理指令
- 算数指令
- 控制转移指令
- 逻辑指令
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
