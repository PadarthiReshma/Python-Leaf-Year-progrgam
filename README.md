# Python-Leaf-Year-progrgam

# Apporach-1
def checkYear(year): 
# Return true if year is a multiple 
# of 4 and not multiple of 100. 
# OR year is multiple of 400. 
	import calendar
	return(calendar.isleap(year)) 	
# Driver Code 
year = 2000
if (checkYear(year)): 
	print("Leap Year") 
else: 
	print("Not a Leap Year") 

 # Apporach-2
 #Variable definition and assignment
year = 2024
if (year % 400 == 0) and (year % 100 == 0):
    print("{0} is a leap year".format(year))
elif (year % 4 ==0) and (year % 100 != 0):
    print("{0} is a leap year.".format(year))
else:
    print("{0} is not a leap year.".format(year))
 # Apporach-3

 year = int(input("Enter a year: "))
if year % 4 == 0:
    if year % 100 == 0:
        if year % 400 == 0:
            print(year, "is a leap year")
        else:
            print(year, "is not a leap year")
    else:
        print(year, "is a leap year")
else:
    print(year, "is not a leap year")

# Apporach-4
# To determine whether a given year is a leap year.
def leap_year(y):
    if y % 400 == 0:
        return True
    if y % 100 == 0:
        return False
    if y % 4 == 0:
        return True
    else:
        return False
print(leap_year(1900))
print(leap_year(2004))

    
    
