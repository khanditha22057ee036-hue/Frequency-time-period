# Frequency and Time Period Calculation

print("Frequency and Time Period Calculator")
print("1. Calculate Time Period")
print("2. Calculate Frequency")

choice = int(input("Enter your choice (1 or 2): "))

if choice == 1:
    frequency = float(input("Enter frequency (Hz): "))

    if frequency > 0:
        time_period = 1 / frequency
        print("Time Period =", time_period, "seconds")
    else:
        print("Frequency must be greater than zero.")

elif choice == 2:
    time_period = float(input("Enter time period (seconds): "))

    if time_period > 0:
        frequency = 1 / time_period
        print("Frequency =", frequency, "Hz")
    else:
        print("Time period must be greater than zero.")

else:
    print("Invalid choice. Please select 1 or 2.")