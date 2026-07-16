import json
import os 
DATA_FILE="students.json"
def load_students():
    """Load student recordsfrom file,if it exists."""
    if os.path.exist(DATA_FILE):
        with open(DATA_FILE,"r") as f:
             return json.load(f)
    return[]
def save_students(students):
    """Save student records to file."""
    with open(DATA_FILE,"W") as f:
        json.dump(students,f, indent=4)
def add_students(students):
    name = input("Enter student name:")
    roll_no = input("Enter roll number:")
    marks = input("Enter marks:")
    students={"name":name,"roll_no":roll_no,"marks":marks}
    students.append(student)
    save_students(students)
    print(f"Student '{name}' added successfully!\n")
def view_students(students):
    if not students:
        print("No student records found.\n")
        return 
    print("\n--- All Students ---")
    for s in students:
        print(f"Roll No: {s['roll_no']} | Name: {s['name']} | Marks: {s['marks]}")
    print()
def search_students(students):
    roll_no = input(roll_no = input("Enter roll number to delete: ")
    for s in students:
        if s["roll_no"] == roll_no:
            students.remove(s)
            save_students(students)
            print(f"Student with roll number {roll_no} deleted.\n")
            return
    print("Student not found.\n")


def main():
    students = load_students()

    while True:
        print("=== Student Management System ===")
        print("1. Add Student")
        print("2. View All Students")
        print("3. Search Student")
        print("4. Delete Student")
        print("5. Exit")

        choice = input("Enter your choice (1-5): ")

        if choice == "1":
            add_student(students)
        elif choice == "2":
            view_students(students)
        elif choice == "3":
            search_student(students)
        elif choice == "4":
            delete_student(students)
        elif choice == "5":
            print("Exiting... Goodbye!")
            break
        else:
            print("Invalid choice. Please try again.\n")


if __name__ == "__main__":
    main()
