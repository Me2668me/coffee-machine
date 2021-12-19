# coffee-machine
Coffee vending machine, select menu, charge
print("---Welcome to Grammy's Coffee---\n")
es = "Espresso" 
ca = "Cappucino"
la = "Latte"
hot = 55
cold = 60
menu = int(input("Please type 1 to show menu: "))
if menu == 1:
    print("\n---Choose the menu---")
    print("1. Espresso\n2. Cappucino\n3. Latte\n")
    coffee = int(input("Select coffee: "))
    if coffee == 1:
        print("1. Hot 55 baht\n2. Cold 60 baht")
    elif coffee == 2:
        print("1. Hot 55 baht\n2. Cold 60 baht")
    elif coffee == 3:
        print("1. Hot 55 baht\n2. Cold 60 baht")
    typecof = int(input("\nSelect type: "))
    if typecof <= 1 and coffee == 1:
      print("---You chose hot %s %d baht---\n" % (es,hot))
    elif typecof <= 1 and coffee == 2:
      print("---You chose hot %s %d baht---\n" % (ca,hot))
    elif typecof <= 1 and coffee == 3:
      print("---You chose hot %s %d baht---\n" % (la,hot))
    elif typecof <= 2 and coffee == 1:
      print("---You chose cold %s %d baht---\n" % (es,cold))
    elif typecof <= 2 and coffee == 2:
      print("---You chose cold %s %d baht---\n" % (ca,cold))
    elif typecof <= 2 and coffee == 3:
      print("---You chose cold %s %d baht---\n" % (la,cold))   
    else:
      print("Sorry, something went wrog")
    money = int(input("Input your money: "))
    if typecof <= 1 and money >= 55 :
      result = money - 55
      print("You recieved a change of %d baht\n---Thank you---" % result)
    elif typecof <= 2 and money >= 60 :
      result = money - 60
      print("You recieved a change of %d baht\n---Thank you---" % result)
    else:
      print("Not enough money\n---Please try again---")
elif menu != 1:
    print("Sorry, something went wrog")                
