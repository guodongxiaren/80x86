DIV/IDIV
=========
- DIV 无符号除法
- IDIV 带符号除法

##DIV
格式：
```asm
div SRC
```
###字节操作
被除数（16位）在**AX**中，除数（8位）为源操作数（SRC），
商（8位）在**AL中**，余数（8位）在**AH**中。
###字操作
被除数（32位）在**AX**中，除数（16位）为源操作数，
商（16位）在**AL中**，余数（16位）在**AH**中。
###双字操作
被除数（64位）在**AX**中，除数（32位）为源操作数，
商（32位）在**AL中**，余数（2位）在**AH**中。
###四字操作
...
##IDIV
格式：
```asm
idiv src
```
**idiv**与**div**相同，但所有操作数、商和余数都是带符号数。
	余数符号和被除数相同
	
