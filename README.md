def length_converter():
    print("Length Converter")
    print("1. Kilometers to Miles")
    print("2. Miles to Kilometers")
    print("3. Centimeters to Inches")
    print("4. Inches to Centimeters")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        km = float(input("Enter distance in kilometers: "))
        miles = km * 0.621371
        print(f"{km} km is equal to {miles} miles")

    elif choice == 2:
        miles = float(input("Enter distance in miles: "))
        km = miles * 1.60934
        print(f"{miles} miles is equal to {km} km")

    elif choice == 3:
        cm = float(input("Enter length in centimeters: "))
        inches = cm * 0.393701
        print(f"{cm} cm is equal to {inches} inches")

    elif choice == 4:
        inches = float(input("Enter length in inches: "))
        cm = inches * 2.54
        print(f"{inches} inches is equal to {cm} cm")

    else:
        print("Invalid choice")

def weight_converter():
    print("Weight Converter")
    print("1. Kilograms to Pounds")
    print("2. Pounds to Kilograms")
    print("3. Grams to Ounces")
    print("4. Ounces to Grams")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        kg = float(input("Enter weight in kilograms: "))
        pounds = kg * 2.20462
        print(f"{kg} kg is equal to {pounds} pounds")

    elif choice == 2:
        pounds = float(input("Enter weight in pounds: "))
        kg = pounds * 0.453592
        print(f"{pounds} pounds is equal to {kg} kg")

    elif choice == 3:
        grams = float(input("Enter weight in grams: "))
        ounces = grams * 0.035274
        print(f"{grams} grams is equal to {ounces} ounces")

    elif choice == 4:
        ounces = float(input("Enter weight in ounces: "))
        grams = ounces * 28.3495
        print(f"{ounces} ounces is equal to {grams} grams")

    else:
        print("Invalid choice")

def temperature_converter():
    print("Temperature Converter")
    print("1. Celsius to Fahrenheit")
    print("2. Fahrenheit to Celsius")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        celsius = float(input("Enter temperature in Celsius: "))
        fahrenheit = (celsius * 9/5) + 32
        print(f"{celsius}°C is equal to {fahrenheit}°F")

    elif choice == 2:
        fahrenheit = float(input("Enter temperature in Fahrenheit: "))
        celsius = (fahrenheit - 32) * 5/9
        print(f"{fahrenheit}°F is equal to {celsius}°C")

    else:
        print("Invalid choice")

def main():
    while True:
        print("Unit Converter")
        print("1. Length")
        print("2. Weight")
        print("3. Temperature")
        print("4. Quit")

        choice = int(input("Enter your choice: "))

        if choice == 1:
            length_converter()
        elif choice == 2:
            weight_converter()
        elif choice == 3:
            temperature_converter()
        elif choice == 4:
            break
        else:
            print("Invalid choice")

if __name__ == "__main__":
    main()

