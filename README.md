# Cafe-Management-System
#CAFE MANAGEMENT SYSTEM
coffee={
    'coca':250,
    'mocha':250,
    'black coffee':250,
    'iced coffe':250,
    'Charcatfire':250,
    'Expresso':300,
    'Cuban':300,
    'latte':300,
}

Toast={
    'cheese Toast':250,
    'Jam Toast':150,
    'Avocados Toast':250,
    'Ham Toast':250,
    'Strawaberry Toast':150,
}

#Greet
print("Welcome to RAMAN CAFE")
print("Coffee")
print("coca:250\nmocha:250\nblack coffee:250\niced coffe:250Charcatfire:250\nExpresso:300\nCuban:300\nlatte:300")
order_total=0
item_1=input("Enter a coffee you want:")
if item_1 in coffee:
    order_total+=coffee[item_1]
    print("Item has been added to your order!")
else:
    print("ordered item is not available yet!")

another_order=input("anything extra to drink:(yes/no)")
if another_order=="yes":
    item_2=input("Enter a coffee you want: ") 
    if item_2 in coffee:
        order_total+=coffee[item_2]
        print("Item has been added to your order!") 
    else:
        ("ordered item is not available yet!")
else:
    print("thankyou for ordering coffee!")
    
toast_2=input("Anything in toast to eat(yes/no)")
if toast_2=="yes":
    print("cheese Toast:250\nJam Toast:150\nAvocados Toast:250\nHam Toast:250\nStrawaberry Toast:150")
    toast_3=input("enter the toast you would like to have")
    if toast_3 in Toast:
        order_total+=Toast[toast_3]
        print("Item is been added to your order")
        another_toast=input(" Anything more you would like to have in toast(yea/no)")
        if another_toast=="Yes":
            toast_extra=input("enter a toast you would like to have:")
            if toast_extra in Toast:
                order_total+=Toast[toast_extra]
                print("Item is been added to you order")
            else:
                print("orderd item is not available!") 
        else:
            print("thankyou for visiting!")
    else:
        print("ordered item is not available yet!")
else:
    print("Thank you for visiting!")


print("Your bill is Rs",order_total)               



