# Python_calculator
Calulator_Code_ For_Daily_Use
def calculator():
    print("--- Simple Python Calculator ---")
    while True:
        print("\nOperations: 1(+), 2(-), 3(*), 4(/), 5(Exit)")
        choice = input("Select (1-5): ")
        if choice == '5': break
        if choice in ('1', '2', '3', '4'):
            try:
                n1 = float(input("First number: "))
                n2 = float(input("Second number: "))
                if choice == '1': print("Result:", n1 + n2)
                elif choice == '2': print("Result:", n1 - n2)
                elif choice == '3': print("Result:", n1 * n2)
                elif choice == '4':
                    print("Result:", n1 / n2 if n2 != 0 else "Error: Div by 0")
            except ValueError: print("Invalid input.")

if __name__ == "__main__":
    calculator()
