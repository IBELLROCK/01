x = []
a = float  
sum = 0
avg = 0
max = 0
min = 0
while a !=0:
    a = float (input('ใส่เดียวได้หมด: '))
    x.append(a) 
del x[-1]
cntsum = len(x)
for i in range (cntsum):
    sum = sum + x[i]
    if x[i] > max:
        max = x[i]

min = sum
for i in range (cntsum):
    if x[i]     < min:
        min = x[i]
        
avg = sum / cntsum

print(x)
print('จำนวนใส่เดียวทั้งหมด = ', cntsum)
print('ผลรวมใส่เดียทั้งหมด = ', sum)
print('ค่าเฉลี่ยใส่เดีย = ', avg)
print('ค่าใส่เดียมากสุด', max)
print('ค่าใส่เดียน้อยสุด', min)

