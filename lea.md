LEA
====
����Ч��ַ����Ĵ���
##ָ���ʽ
```asm
;Intel
lea DEST��SRC
;AT&T
leal SRC, DESC
leaw SRC, DESC
leab SRC, DESC
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