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

## Chapter 3: Conditions: if, then, else

### Is Positive
```.py
a = int(input())

if a > 0:
    print("YES")
    
else:
    print("NO")
```
![](z3_1.png)

### Is odd
```.py
a = int(input())

if a % 2 == 1:
    print("YES")
else:
    print("NO")
```
![](z3_2.png)

### Is even
```.py
a = int(input())

if a % 2 == 1:
    print("NO")
else:
    print("YES")
```
![](z3_3.png)

### Ends on seven
```.py
a = int(input())

if a % 10 == 7:
    print("YES")
else:
    print("NO")
```
![](z3_4.png)

### Minimum of two numbers
```.py
a = int(input())
b = int(input())

if  a < b:
    print(a)
else:
    print(b)
```
![](z3_5.png)

### Are both odd
```.py
a = int(input())
b = int(input())

if a % 2 == 0 or b % 2 == 0:
    print("NO")
else:
    print("YES")
```
![](z3_6.png)


### At least one odd
```.py
a = int(input())
b = int(input())

if a % 2 == 1 or b % 2 == 1:
    print("YES")
else:
    print("NO")
```
![](z3_7.png)


### Exactly one odd
```.py
a = int(input())
b = int(input())

if a % 2 == 1 and b % 2 == 0:
    print("YES")
else:
    if b % 2 == 1 and a % 2 == 0:
        print("YES")
    else:
        print("NO")
```
![](z3_8.png)


### Sign function
```.py
a = int(input())

if a > 0:
    print("1")
elif a < 0:
    print("-1")
else:
    print("0")
```
![](z3_9.png)


### Numbers in ascending order
```.py
a = int(input())
b = int(input())
c = int(input())

if a > b:
    print("NO")
elif b > c:
    print("NO")
else:
    print("YES")
```
![](z3_10.png)

### Is three digits
```.py
a = int(input())

if a < 100:
    print("NO")
elif a > 999:
    print("NO")
else:
    print("YES")
```
![](z3_11.png)

### Minimum of three numbers
```.py
a = int(input())
b = int(input())
c = int(input())

if b > a and c > a:
    print(a)

elif a > b and c > b:
    print(b)
    
else:
    print(c)
```
![](z3_12.png)

### Equal numbers
```.py
a = int(input())
b = int(input())
c = int(input())

if a == b == c:
    print("3")
elif a == b or b == c or c == a:
    print("2")
else:
    print("0")
```
![](z3_13.png)

### Rook move
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

if a == c and b == d or b == c and a == d:
    print("NO")
    
elif a == c or a == d or b == c or b == d:
    print("YES")
```
![](z3_14.png)

### Chess board - black square
```.py
a = int(input())
b = int(input())

aa = a + b

if aa % 2 == 0:
    print("BLACK")
else:
    print("WHITE")
```
![](z3_15.png)


### Chess board - same color
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

aa = a + b
bb = c + d

if aa % 2 == 0 and bb % 2 == 0:
    print("YES")
else:
    if aa % 2 == 1 and bb % 2 == 1:
        print("YES")
    else:
        print("NO")
```
![](z3_16.png)

### Distance to the cloest point
```.py
a = int(input())
b = int(input())
c = int(input())

x = abs(a - b)
y = abs(a - c)

if x > y:
    print(y)
else:
    print(x)
```
![](z3_17.png)

### Digits in ascending order
```.py
a = int(input())

x = a // 100
y = (a // 10) % 10
z = (a % 100) % 10

if x < y < z:
    print("YES")
else:
    print("NO")
```
![](z3_18.png)

### Four-digit palindrome
```.py
a = int(input())

w = a // 1000
x = (a // 100) % 10
y = (a // 10) % 10
z = (a % 100) % 10

if w == z and x == y:
    print("YES")
else:
    print("NO")
```
![](z3_19.png)

### King move
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

if -2 < (a - c) <2 and -2 < (b - d) <2:
    print("YES")
else:
    print("NO")
```
![](z3_20.png)

### Bishop move
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

x = (a - c) 
y = (b - d) 
z = (d - b)

if x == y or x == z:
    print("YES")
else:
    print("NO")
```
![](z3_21.png)

### Queen move
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

x = (a - c) 
y = (b - d) 
z = (d - b)

if x == y or x == z or a == c or b == d:
    print("YES")
else:
    print("NO")
```
![](z3_22.png)








