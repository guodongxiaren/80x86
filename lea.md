LEA
====
将有效地址送入寄存器
##指令格式
```asm
;Intel
LEA DEST，SRC
;AT&T
LEAL SRC, DESC
LEAW SRC, DESC
LEAB SRC, DESC
```
- SRC可以是除~~立即数~~和~~寄存器~~外的任一种存储器寻址方式。   
- DESC可以是寄存器，但不能是~~段寄存器~~

在**AT&T**语法中，该指令需要加后缀（q、l、w、b）来表示操作数的大小
##栗子
```asm
;Intel
lea eax [esp+28]
;AT&T
leal 28(%esp) %eax
```
将栈中esp+28位置的有效地址（而非该位置的储存的值）传递给eax。