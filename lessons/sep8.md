```.py
#First Activity
a = int(input("enter the number"))
b = 1
c = 0

while b < a:
    if a % b == 0:
        print(b)
        c += b
    b += 1
print(f'the sum of the factor is {c}')
if a == c:
    print('True')
else:
    print('False')

#-----------------------------------------------------------

x = [[3, 8], ["bab", "30"], 5, "alice"]

index= 0
a = 0


while index < len(x):
    print(f"Item #{index}: {x[index]}")
    index += 1


for i in x:
   print(f"Item #{a}: {i}")
   a += 1

#-----------------------------------------------------------

numbers = []
numbers = list()
value = 0

while value < 10:
    numbers.append(value)
    print(numbers)
    value += 1
    
```
