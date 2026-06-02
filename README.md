# Expense-tracker
expenses= []
while True:
    print("1=add expense")
    print("2=review all expenses")
    print("3=calculate total expenses")
    print("4=exit")

    choice = input("Enter the choice: ")
    if choice == "1":
       category = input('Enter the catagory:')
       amount = int(input("Enter expense: "))
       expenses.append({"category": category, "amount": amount})
       print(expenses)

    elif choice == "2":
         print(expenses)

    elif choice == "3":
        total= sum(item["amount"] for item in expenses) 
        print(total)
    elif choice == "4":
        break
    else:
        print("Enter a valid choice")