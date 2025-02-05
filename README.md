# Magic-Lab
print("WELCOME TO THE MAGIC LAB")
def determine_solution_type(pH):
    # Check if the pH value is within the valid range
    if pH < 0 or pH > 14:
        return "NICE TRY , KEEP GUESSING YOU'RE GETTING CLOSER . THE CLUE IS THE PH RANGE ."
    elif pH < 7:
        return "The magic solution is Acid.  "
    elif pH == 7:
        return "The magic solution is Neutral. "
    else:
        return "The magic solution is Base."

# Main Program
try:
    pH_value = float(input("Can you guess the mysterious code : "))
    result = determine_solution_type(pH_value)
    print(result)
except ValueError:
    print("Nice try ! Try to guess the secret code.")
