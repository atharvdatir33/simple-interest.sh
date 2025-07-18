# simple-interest.sh
# simple_interest.py

def calculate_simple_interest(principal, rate, time):
    """
    Calculate simple interest using the formula:
    SI = (P * R * T) / 100
    """
    return (principal * rate * time) / 100


def main():
    print("Simple Interest Calculator")
    try:
        principal = float(input("Enter the Principal Amount: "))
        rate = float(input("Enter the Rate of Interest: "))
        time = float(input("Enter the Time (in years): "))

        si = calculate_simple_interest(principal, rate, time)
        print(f"\nSimple Interest = {si:.2f}")
        total_amount = principal + si
        print(f"Total Amount = {total_amount:.2f}")
    except ValueError:
        print("Please enter valid numeric inputs.")


if __name__ == "__main__":
    main()
