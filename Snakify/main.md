# Snakify
## Chapter 1: Input, print and numbers

### Sum of three numbers
```.py
a = int(input())
b = int(input())
c = int(input())
print(a + b + c)
```
![](z1_1.png)

### Hi John
```.py
name = input()
print('Hi', name)
```
![](z1_2.png)

### Square
```.py
num = int(input())
print(num ** 2)
```
![](z1_3.png)

### Area of right-angled triangle
```.py
length = int(input())
height = int(input())

print(float(length*height/2))
```
![](z1_4.png)

### Hello, Harry!
```.py
name = input()

print('Hello, ' + name + '!' )
```
![](z1_5.png)

### Apple sharing
```.py
n = int(input())
k = int(input())

print(k // n)
print(k % n)
```
![](z1_6.png)

### Previous and next
```.py
a = int(input())

b = str(a + 1)
c = str(a - 1)

print('The next number for the number ' + str(a) + ' is ' + str(b) + '.')
print('The previous number for the number ' + str(a) + ' is ' + str(c) + '.')
```
![](z1_7.png)

### Two timestamps
```.py
a1 = int(input())
a2 = int(input())
a3 = int(input())
b1 = int(input())
b2 = int(input())
b3 = int(input())

print(b1*3600 + b2*60 + b3 - a1*3600 - a2*60 - a3)
```
![](z1_8.png)

### School desks
```.py
class_a = int(input())
class_b = int(input())
class_c = int(input())

print(class_a // 2 + class_a % 2 + class_b // 2 + class_b % 2 + class_c // 2 + class_c % 2)
```
![](z1_9.png)

## Chapter 2: Integer and float numbers

### Last digit of integer
```.py
a = int(input())

print(a%10)
```
![](z2_1.png)

### Two digits
```.py
a = int(input())

print(a // 10, a % 10)
```
![](z2_2.png)

### Swap digits
```.py
a = int(input())

b = a%10
c = a//10
print(b*10 + c)
```
![](z2_3.png)

### Last two digits
```.py
a = int(input())

b = a % 100

print(b)
```
![](z2_4.png)

### Tens digit
```.py
a = int(input())

print(a // 10 % 10)
```
![](z2_5.png)

### Sum of digits
```.py
a = int(input())

print(a // 100 + a // 10 % 10 + a % 10)
```
![](z2_6.png)

### Reverse three digits
```.py
a = int(input())

b = a // 100
c = a // 10 % 10 * 10
d = a %10 * 100
print(b + c + d)
```
![](z2_7.png)


### Merge two numbers
```.py
a = int(input())
b = int(input())

a1 = a // 10 * 1000
a3 = a % 10 * 10
b2 = b // 10 * 100
b4 = b % 10

print(a1 + b2 + a3 + b4)
```
![](z2_8.png)

### Cyclic rotation
```.py
a = int(input())

a1 = a // 1000 * 10
a2 = a // 100 % 10
a3 = a // 10 % 10
b1 = a3 *1000
a4 = a % 10 * 100

print(a1 + a2 + b1 + a4)
```
![](z2_9.png)

### Fractional Part
```.py
a = float(input())

print(a - int(a))
```
![](z2_10.png)

### First digit after decimal point
```.py
b = float(input())

a = b *10
c = a %10

print(int(c))
```
![](z2_11.png)

### Car route
```.py
n = int(input())
m = int(input())

a = m / n
b = m // n

if a == int(a):
    print(a)
    
else:
    print(b + 1)
```
![](z2_12.png)

### Day of week
```.py
a = int(input())

b = (a + 3) % 7

print(b)
```
![](z2_13.png)

### Digital clock
```.py
a = int(input())

b = a // 60

c = a % 60

print(b,c)
```
![](z2_14.png)

### Total cost
```.py
a = int(input())
b = int(input())
n = int(input())

aa = a*n
bb = b*n
cc = bb // 100
dd = bb % 100

if bb > 100:
    bb = dd
    aa += cc

print(aa,bb)
```
![](z2_15.png)

### Century
```.py
a = int(input())

b = a // 100

if a % 100 == 0:
    print(a // 100)
else:
    print(b + 1)
```
![](z2_16.png)

### Snail
```.py
from math import ceil

h = int(input())
a = int(input())
b = int(input())
print(ceil((h - a) / (a - b)) + 1)
```
![](z2_17.png)

### Clock face - 1
```.py
from math import ceil

h = float(input())
m = float(input())
s = float(input())

a = h*30
b = m*0.5
c = s*(30/3600)
print(a + b + c)
```
![](z2_18.png)

### Clock face - 2
```.py
a = float(input())

b = a % 30

print(b*12)
```
![](z2_19.png)











