






student = {}

while True:
    print("\n-----STUDENT MANAGEMENT SYSTEM-----")
    print("1. Add Student")
    print("2. View Students")
    print("3. Check Results")
    print("4. Exit")
    choice = input("Enter your choice:")

    if choice == "1":
        name = input("Enter student name:")
        mark = float(input("Enter student marks:"))
        student[name] = mark
        print(f"student {name} successfully added")

    elif choice == "2":
        if not student:
            print("No students found.")
        else:
            print("\n-----STUDENT RECORDS-----")
            for name, marks in student.items():
                print(f"Name: {name}, Marks: {marks}")

# check results
    elif choice =="3":
      name = input("Enter student name to check result:")
    if name in student:
        marks = student[name]
        if marks >= 40:
            print(f"{name} has passed with marks {marks}")
        else:
            print(f"{name} student not found")
        # choice 4

    elif choice == "4":
        print("Exiting.")
        break
    else:
        print("Invalid option. Please enter 1-4.")







student = {}

while True:
    print("\n-----STUDENT MANAGEMENT SYSTEM-----")
    print("1. Add Student")
    print("2. View Students")
    print("3. Check Results")
    print("4. Exit")
    choice = input("Enter your choice:")

    if choice == "1":
        name = input("Enter student name:")
        mark = float(input("Enter student marks:"))
        student[name] = mark
        print(f"student {name} successfully added")

    elif choice == "2":
        if not student:
            print("No students found.")
        else:
            print("\n-----STUDENT RECORDS-----")
            for name, marks in student.items():
                print(f"Name: {name}, Marks: {marks}")

# check results
    elif choice =="3":
      name = input("Enter student name to check result:")
    if name in student:
        marks = student[name]
        if marks >= 40:
            print(f"{name} has passed with marks {marks}")
        else:
            print(f"{name} student not found")
        # choice 4

    elif choice == "4":
        print("Exiting.")
        break
    else:
        print("Invalid option. Please enter 1-4.")
