names = []
phone_numbers = []
num = int(input("enter num of numbers you want to input:"))
for i in range(num):
    name=input("Name:")
    phone_number = input("phone_Number:")
    names.append(name)
    phone_numbers.append(phone_number)
    print("\nName\t\t\phone_Number\n")
    for i in range(num):
        print("{}\t\t\t{}".format(names[i],phone_numbers[i]))
        search_term = input("\n enter search term:")
        print("Search result:")
    if search_term in names:
            index= names.index(search_term)
            phone_numbers=phone_numbers[index]
            print("Name:{},phone_number:{}".format(search_term,phone_number))
    else:
        print("Name not found")
