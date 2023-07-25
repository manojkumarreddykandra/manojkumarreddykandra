- 👋 Hi, I’m @manojkumarreddykandra
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
manojkumarreddykandra/manojkumarreddykandra is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
def grade_calculator(marks):
  """
  Calculates and returns the grade for a student based on the marks obtained.

  Args:
    marks: The marks obtained by the student.

  Returns:
    The grade for the student.
  """
  if marks >= 90:
    grade = "A+"
  elif marks >= 80:
    grade = "A"
  elif marks >= 70:
    grade = "B"
  elif marks >= 60:
    grade = "C"
  elif marks >= 50:
    grade = "D"
  else:
    grade = "Fail"
  return grade


def main():
  """
  The main function of the program.

  This function prompts the user to enter the marks for a student and then calculates and displays the grade for the student.
  """
  while True:
    marks = float(input("Enter the marks obtained by the student: "))

    # Check if the marks are valid.
    if marks < 0 or marks > 100:
      print("Invalid marks. Please enter a number between 0 and 100.")
      continue

    grade = grade_calculator(marks)
    print("The grade for the student is:", grade)

    # Ask the user if they want to calculate the grade for another student.
    user_input = input("Do you want to calculate the grade for another student? (Y/N): ")
    if user_input == "N":
      break


if __name__ == "__main__":
  main()
