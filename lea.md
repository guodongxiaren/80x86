LEA
====
����Ч��ַ����Ĵ���
##ָ���ʽ
```asm
;Intel
LEA DEST��SRC
;AT&T
LEAL SRC, DESC
LEAW SRC, DESC
LEAB SRC, DESC
```
- SRC�����ǳ�~~������~~��~~�Ĵ���~~�����һ�ִ洢��Ѱַ��ʽ��   
- DESC�����ǼĴ�������������~~�μĴ���~~

��**AT&T**�﷨�У���ָ����Ҫ�Ӻ�׺��q��l��w��b������ʾ�������Ĵ�С
##����
```asm
;Intel
lea eax [esp+28]
;AT&T
leal 28(%esp) %eax
```
��ջ��esp+28λ�õ���Ч��ַ�����Ǹ�λ�õĴ����ֵ�����ݸ�eax��