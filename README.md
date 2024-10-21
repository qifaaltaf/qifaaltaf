#Programe to input electricity unit charges and calculate total electricity bill:
#Code by :Qifa altaf
unit=int(input("Enter units consumed:"))

if (unit <= 50) :
    amount=unit*0.5
    print("Amount to be paid is",amount)
elif (unit <= 150):
    amount = (50*0.5) + ((unit-50)*0.75)
    print('Amount to be paid is:',amount)

elif (unit <= 250) :
    amoumt = (50*0.5) + (100*0.75) + ((unit-150)*1.20)
    print('Amount to be paid is:', amount)
else:
    amount = (50*0.5) + (100*0.75) + (100*1.2) + ((unit-250)*1.50)
    surcharge = amount*0.20
    total_amt = amount+surcharge
    print('Amount to be paid is:',total_amt)
