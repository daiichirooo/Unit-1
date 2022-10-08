# Cryptowallet

# Criteria A: Planning
## Problem definition
Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics.

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

## Proposed Solution
Design statement: I will design and make a electronic ledger for a client who is Ms.Sato. The electronic ledger will be about recording the customers' economic activity and is constructed using the software FLOW. It will take couple of weeks to make and will be evaluated according to the criteria below.

** add a description of your coin and citation **

『Flow is a fast, decentralized, developer-friendly blockchain designed as the foundation for a new generation of games, apps, and the digital assets that power them. Flow is the only layer-one blockchain developed independently by the team that has consistently delivered superior blockchain experiences for consumers, including, CryptoKitties, Dapper Wallet, and NBA Top Shot.』 (coinmarketcap.2022)





## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal). 
2. The electronic ledger display the basic description of the cyrptocurrency selected. 
3. The electronic ledger allows to enter, withdraw and record transactions. 
4. The electronic ledger can be opened by only client. 
5. The electronic ledger can make a lot of acounts for a lot of people.
6. The electronic ledger suggests whether you spend too much money or not. 

# Criteria B: Design
## System Diagram
![](sd.png)
## Flow Diagrams
### Login
![](fd.png)
### Register
![](ref.png)
### Activate
![](activate.png)
## Record of Tasks
Task No	Planned Action	Planned Outcome	Time estimate	Target completion date	Criterion



| Task Number | Planned Actions | Planned Outcome | Time Estimate | Target Completion Date | Criterion |
|-------------|-----------------|-----------------|---------------|------------------------|-----------|
|1            |Create system diagram|To have a clear idea of the hardware and software requirements for the proposed solution|10m|Sep 24|B|
|2            |Create a login function|To ensure that only users can log in.|5h|Sep 27|C|
|3            |Create a register function|To allow multiple users to use this service.|5h|Sep 29|C|
|4            |Create a activate function|To have users make deposits and withdrawals and see their records.|1w|Oct 6|C|
|5            |Make program hashes a data in csv file|To protect the user's personal information.|2h|Oct 6|C|
|6            |Test all the code|To make sure that everything works well.|20m|Oct 7|C|
|7            |Draw Flow Diagram|A flow diagram of the program's functionality must be completed.|20m|Oct 8|C|
|8            |Write the Github|To complete the assignment|3h|Oct 9|C|

# Criteria C: Development
## Login System
my client requires a system to protect the private data. I thought about using a login system to accomplish this requirement using a if condition and the open command to work with a CSV file. more description of the code...

```.py
def login(user:str, password:str)->bool:
    '''
    Fanction for a simple user login needs db.csv
    :param user: string
    :param password: string
    :return: True or False
    '''
    with open("crypto_projects/db.csv") as file:
        database = file.readlines()

    output=False
    for line in database:
        clear_line = line.strip()
        separated_line = clear_line.split(",")
        if user == separated_line[0] and password == separated_line[1]:
            output = True


    return output

```

my client requires a system whether the user is a new user or not.  I thought about using a register system to accomplish this requirement using the open command to work with a CSV file.

```.py
def register(newuname:str, newpassword:str):
    '''
    This function saves a user, password in the file
    db.csv
    :param uname: username a string
    :param password: password a string
    :return: nothing
    '''

    #Open the file in mode append:a
    #this means, add to the end of the file

    file = open("crypto_projects/db.csv", "a")
    file.write(f"{newuname},{newpassword}\n")
```
