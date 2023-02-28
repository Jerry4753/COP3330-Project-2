**COP3330-Project-2**
**NOTE:** Due to professor's grading preference, all classes are in one .java file, though this is not best practice

**Project 2 statement**
Please read this entire statement carefully before you start doing anything...
This project involves implementing a simple university personnel management program. The program contains three kinds 
of objects: Staff, student and faculty. For each object, the program stores relevant information such as university ID, name, 
etc. Different information is stored depending on the type of the object. For example, a student has a GPA, a faculty has a 
title and department (professor, mathematics).
For each of any class data member, your program must include the getters and the setters, and each class must include at 
least two constructors. The goal of this Project is to demonstrate the use of inheritance, abstract classes, abstract methods, 
and method overriding. 
For a student, we need a:
- full name 
- id
- gpa
- Number of credit hours currently taken
For a faculty, we need a:
- full name
- id
- department (mathematics, engineering or english)
- Rank (professor or adjunct)
For a staff, we need a:
- full name
- id
- department (mathematics, engineering or english)
- status (part time or full time)
Students in this college pay $236.45 per credit hour in addition to a $52 administrative fee. Your code should generate a 
tuition invoice ( a method within the class Student). Note that students get a 25% off total payment if their gpa is greater or 
equal to 3.85.
Your code should implement the following inheritance hierarchy:
Person
Student Employee
Faculty Staff
Both classes Student and Employee inherit from the abstract class Person. The abstract class Person has what is common 
to a Student and an Employee (Faculty or Staff). The class Person must include the signature: public abstract void print();
The abstract method print is overridden to print the fee invoice for a student and to print the information for  a faculty or 
a staff member. It is left to you (the programmer) to come out with other abstract methods if you see fit(this is optional).
The class Employee should also be abstract, and it is supposed to include what is common to a staff and a faculty.
Test your code with ONE array of size 100 of type Person (It must be an array, not an arraylist, linked list , hash map or 
anything else...). The sample run below should give you a clear idea about how your code should run. The user’s entry is 
marked in bold so you can tell what your code should display to the screen and what the user enters.
Please note well that:
1) Your code should run exactly as shown on the sample run below (However, the TA will not deduct points because you 
skipped two lines instead of three or your tuition invoice has 56 hyphens instead of 63 ).
2) When asked to enter the faulty’s department, matheMatics and MathematiCs are  considered to be the same, and your 
program should display Mathematics if faculty information is to be displayed to the screen. However, if the user enters 
Mathematics department, then this is an invalid entry.  Consider theses departments only: Mathematics, Engineering 
and Sciences. As for the rank of a faculty, consider theses ranks only: Professor and Adjunct.
3) The university ID has no required form so you may choose to enter anything to be the ID.
