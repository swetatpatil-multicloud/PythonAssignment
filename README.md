# PythonAssignment
## Question number 1 > Strong password Coding 




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

# --- Output Screenshot ---

<img width="943" height="432" alt="image" src="https://github.com/user-attachments/assets/f272310e-3a4d-4923-ae3e-ca942385a8a6" />


--------------

## Question 2 > CPU-Health

# CPU Health Monitor

A Python script to continuously monitor CPU usage on your local machine.  
If the usage exceeds a predefined threshold (default: 80%), an alert is displayed.  
This tool is ideal for DevOps engineers to track server performance in real time.

## Features

- Monitors CPU usage every second
- Alerts when usage exceeds a set threshold
- Runs indefinitely until manually stopped
- Handles errors gracefully

## How It Works

The script uses the `psutil` library to fetch CPU usage percentage.  
It checks usage at regular intervals and prints an alert if the threshold is crossed.

# Output Screenshot

<img width="931" height="353" alt="image" src="https://github.com/user-attachments/assets/12c7d132-b686-4eb5-89ed-fb3b52b87ce2" /> 

----------
# Question 4 > Backup Files

# Backup Script

A simple Python script to perform regular backups of important files.  
It copies all files from a source directory to a destination directory.  
If a file with the same name already exists in the destination, a timestamp is added to ensure uniqueness.

## Features
- Copies all files from source → destination
- Appends a timestamp if a file already exists
- Skips folders (only copies files)
- Simple and beginner-friendly code

## How It Works
The script loops through files in the source directory and copies them to the destination.  
If a file already exists in the destination, the script renames the new copy with a timestamp.

# Output Screenshot

<img width="932" height="107" alt="image" src="https://github.com/user-attachments/assets/22fa83b8-cf55-4e61-ae0c-bbc2cd662927" />



