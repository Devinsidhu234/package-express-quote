# Welcome message
print("Welcome to Package Express. Please follow the instructions below.")

# Prompt user for the package weight
weight = float(input("Please enter the package weight: "))

# Check if the weight is greater than 50
if weight > 50:
    print("Package too heavy to be shipped via Package Express. Have a good day.")
else:
    # Prompt user for the package dimensions
    width = float(input("Please enter the package width: "))
    height = float(input("Please enter the package height: "))
    length = float(input("Please enter the package length: "))

    # Check if the total dimensions are greater than 50
    if (width + height + length) > 50:
        print("Package too big to be shipped via Package Express.")
    else:
        # Calculate the shipping quote
        volume = width * height * length
        quote = (volume * weight) / 100

        # Display the quote formatted as a dollar amount
        print(f"Your estimated total for shipping this package is: ${quote:.2f}")
        print("Thank you!")
git remote add origin https://github.com/Devinsidhu234/package-express-quote.git
