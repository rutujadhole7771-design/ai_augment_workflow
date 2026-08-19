# ai_augment_workflow
print("================================")
print("     STUDENT GRADE ASSISTANT")
print("================================")

name = input("Enter student name: ")

try:
    marks = float(input("Enter marks out of 100: "))

    if marks < 0 or marks > 100:
        print("Please enter marks between 0 and 100.")

    elif marks >= 90:
        grade = "A+"
        message = "Excellent performance!"

    elif marks >= 80:
        grade = "A"
        message = "Very good performance!"

    elif marks >= 70:
        grade = "B"
        message = "Good performance!"

    elif marks >= 60:
        grade = "C"
        message = "Keep improving!"

    elif marks >= 50:
        grade = "D"
        message = "More practice is needed."

    else:
        grade = "F"
        message = "You need to work harder."

    if 0 <= marks <= 100:
        print("\n----- RESULT -----")
        print("Student:", name)
        print("Marks:", marks)
        print("Grade:", grade)
        print("Feedback:", message)

except ValueError:
    print("Invalid input. Please enter a number for marks.")
