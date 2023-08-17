# Task-2-internpe---shutdown-project-
import os

def shutdown():
    os.system("shutdown /s /t 1")

def restart():
    os.system("shutdown /r /t 1")

def logout():
    os.system("shutdown /l")

while True:
    print("Choose an option:")
    print("1. Shutdown")
    print("2. Restart")
    print("3. Logout")
    print("4. Exit")
    
    choice = input("Enter your choice: ")
    
    if choice == "1":
        shutdown()
    elif choice == "2":
        restart()
    elif choice == "3":
        logout()
    elif choice == "4":
        break
    else:
        print("Invalid choice. Please enter a valid option.")
