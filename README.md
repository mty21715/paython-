# paython-
ship= 12.99
c=0
prodCodeA=9
prodCodeB=21.50
print("\tHello Prof Honda Welcome to my program ")
id= int(input("Enter the customer ID"))
while not ( id==-999):
    prod= input(" Enter The product A for chip or B for pinpaple")
    if prod == 'A':
        qly= int(input("Enter the Quontity "))
        size= int(input("Enter the size for small 1 or 2 for Large "))
        cost= prodCodeA * qly*size
    else:
        if prod=='B':
            qly = int(input("Enter the Qountity "))
            size= int(input("Enter the size for small 1 or 2 for Large "))
            cost = prodCodeB * qly * size
       # else:
        #    print ("you have wrong entry ")
            #endIf
        #endIF
        
    tax=cost*0.04
    finalCost =cost + tax + ship
    c=c+1
    print("Customer id = ",id,"cost of order ", finalCost,"counter",c)
    id = int(input("Enter customer ID"))
    #endWhile
print("End of the program")
