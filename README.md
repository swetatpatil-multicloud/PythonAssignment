<!-- # PythonAssignment -->

def check_password_strength(password):
    # Check minimum length
    if len(password) < 8:
        return False

    # Flags for each condition
    has_upper = False
    has_lower = False
    has_digit = False
    has_special = False

    # Check each character
    for char in password:
        if char.isupper():
            has_upper = True
        elif char.islower():
            has_lower = True
        elif char.isdigit():
            has_digit = True
        elif char in "!@#$%^&*()_+-=[]{};:'\",.<>?/\\|":
            has_special = True

    # Return True only if all conditions are met
    return has_upper and has_lower and has_digit and has_special


# --- Main Program ---
user_password = input("Enter your password: ")

if check_password_strength(user_password):
    print("✅ Strong password! Meets all security criteria.")
else:
    print("❌ Weak password. Please include:")
    print("- At least 8 characters")
    print("- Uppercase and lowercase letters")
    print("- At least one digit")
    print("- At least one special character (!, @, #, $, %)")


    ![CPU Monitor Output](images/cpu_monitor_output.png)
