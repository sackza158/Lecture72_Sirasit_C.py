menuList = []

priceList = []


def showBill():

    totalPrice = 0
    
    textShowmenu = "My Food"
    
    print(textShowmenu.center(21,"-"))
    
    for number in range(len(menuList)):
    
        print(menuList[number])
        
        totalPrice += int(menuList[number][1])
        
    print("Total Price(THB) :",totalPrice)
    

while True:

    menuName = input("Plese Enter Menu :")
    
    if(menuName.lower() == "exit"):
    
        break
        
    else:
    
        menuPrice = input("Price :")
        
        menuList.append([menuName, menuPrice])
        

showBill()
