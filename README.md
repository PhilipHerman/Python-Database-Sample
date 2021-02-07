# Python-Database-Sample
A database created with Python that lets you check if a student is on the honor roll or academic probation.


App.py

from Student import Student

student1 = Student("Oscar", "Accounting", 3.1)
student2 = Student("Phyllis", "Business", 3.8)
student3 = Student("Derek", "Computer Science", 1.7)
student4 = Student("Alex", "Marketing", 2.7)
student5 = Student("Jordan", "Accounting", 3.8)
student6 = Student("Max", "Nursing", 4.0)
student7 = Student("Andrew", "Computer Science", 3.7)
student8 = Student("Austin", "Pharmacy", 3.0)
student9 = Student("Stephen", "Business", 1.9)
student10 = Student("Blake", "Engineering", 2.1)

print(student9.on_honor_roll())







Student.py
class Student:
    def __init__(self, name, major, gpa):
        self.name = name
        self.major = major
        self.gpa = gpa

    def on_honor_roll(self):
        if self.gpa >= 3.5:
            return True
        else:
            return False

    def on_deans_list(self):
        if self.gpa >= 4.0:
            return True
        else:
            return False

    def on_academic_probation(self):
        if self.gpa >= 2.0:
            return True
        else:
            return False

