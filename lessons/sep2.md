```.py
salary = int(input("Enter you salary"))

if salary < 10000:
    tax = salary* 0.05

else:
    if 10001 < salary < 50000:
        tax = salary* 0.1
    else:
        if 50001 < salary < 100000:
            tax = salary* 0.15
        else:
            if 100001 < salary:
                tax = salary* 0.25

print(f"Your tax is {tax} USD. Please pay as soon as you can.")

```

![The photo of the result]()
