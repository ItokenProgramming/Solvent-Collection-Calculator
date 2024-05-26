# 回収溶媒計算ソフト


詳細は[こちら](https://github.com/ItokenProgramming/Solvent-Collection-Calculator/raw/main/About-Solvent-Collection-Calculator.pdf)を参照されたい。ソースコードを以下に示す。

```
"VOLUM SUM="?→V
"KAISHU H/E="?→K
"IDEAL H/E="?→A
CLS
LOCATE 1,1,"KAISHU="
IF B<A:THEN LOCATE 8,1,V*(K+1)/(A+1):LOCATE 1,2,"HEXANE=":LOCATE 8,2,V-V*(K+1)/(A+1):LOCATE 15,1,"ML":LOCATE 15,2,"ML"
ELSE LOCATE 8,1,V/(1/A-1/(A*(K+1))-1/(K+1)+1):LOCATE 1,2,"ETAC=":LOCATE 8,2,V-V/(1/A-1/(A*(K+1))-1/(K+1)+1):LOCATE 15,1,"ML":LOCATE15,2,"ML"
IFEND:ANS
```
