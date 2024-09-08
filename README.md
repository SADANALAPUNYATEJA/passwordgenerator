
import random as r
uppercase_letter="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
lowercase_letter=uppercase_letter.lower()
digits="0123456789"
symbols="@/\#_+()[]{,;:,.}"
upper,lower,num,sym=True,True,True,True
all=""
if lower:
    all+=lowercase_letter
if upper:
    all+=uppercase_letter
if num:
    all+=digits
if sym:
    all+=symbols

len=20
amount=10

for x in range(amount):
     password=" ".join(r.sample(all,len))
     print(password)
