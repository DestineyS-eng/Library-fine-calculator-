#A library needs a program to calculate fines for overdue books.
overdue=int(input("how many days is your book overdue:"))
if overdue>=1 and overdue<=7:
    #if its between 1 and 7 days then the fine is £0.5 per day
    fine=0.5*overdue
    print(fine)
elif overdue>7:
    #if book is overdue for more than a week charge for the frist week as £3.50 then add individual days after that week for £1
    fine2=overdue-7
    #price for days after a week 
    fine=3.50
    #price for one week
    total=fine2+fine
    print(total)
else:
    print("you aren't overdue")
    # alternative root for books that are at 0 days overdue 
    
