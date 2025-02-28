# Exam1 Supplemental Assignment
## Assignment Goal 
A simple Java program using File IO and linked lists.
## Team Work 
No team work is allowed. Work individually. You cannot discuss the 
assignment with ANYONE other than the instructor and discussion board. 
## Programming Language 
You are required to program using Java. 
## Compilation Method 
Compilation: Your code should compile on vsphere or online gdb 
## Policy on sharing of code 
 EVERY line of code that you submit in this assignment should be written by you. Do NOT show your code to any other student. Do not copy any code from any online source. Code for File I/O or String operations, if found online, should be clearly cited, and you cannot use more than 5 lines of such online code. 

Code snippets, for File I/O, if used from an online source should be cited by mentioning it in the README.md and also in the documentation of every source file in which that code appears. 

 Post to the BrightSpace discussion if you have any questions about the requirements. Do NOT post your code asking for help with debugging. 
## Project Description 
### Assignment Goal: Develop a program, using Java, to accumulate attendance and handle excused absences. 

(1) First create an attendance linked list from the first file by creating a DayNode such that the node contains a pointer to the next node and as for the data include the date, and students for that day. The information for DayNode can be extracted from the first file, assuming there exists at maximum 20 students per day.

(2) Subsequently, use the attendance linked list to create a student list of type StudentNode such that each node contains the pointer to the next node and as for the data include the name, number of classes attended, and explanations. Assume you use the attendance list to populate the student list and extract the name and number of classes attended.

(3) Next, use the second file to update the matching student node from the list by 1 day of class attended and the explanation. Concatenate explanations with the respective date.

(4) Finally, write the student node list to the third file with the contents of each code separated by comma values on each line.

## INPUT FORMAT (attend_sheet.txt)
```
<date> <student_0> <student_1> <student_2> <student_n-1>
```

### INPUT EXAMPLES 
```
1/21 John Doe Jane Doe Jason X
1/23 Jane Doe George W Jackson A 
```

## INPUT FORMAT (absense_sheet.txt)
```
<date>, <student_0> ,<reason_0>
```

### INPUT EXAMPLES (absense_sheet.txt)
```
1/21 John Doe, “Called out to military service”
1/23 Jane Doe, “Job Interview”
1/25  John Doe, “Sickness”
```

### OUTPUT FORMAT (student_attendance_book.csv)
Your program should write to an output file called 
```
<student_0>,<classes_attended>,<explanations> 
<student_1>,<classes_attended>,<explanations> 
<student_2>,<classes_attended>,<explanations> 
```

## OUTPUT EXAMPLES 
```
John Doe, 23, “Called out to military service (1/21), Sickness (1/25)”
Jane Doe, 23, “Job Interview (1/23)”
```

## NOTES ON GRADING 
Points will be given to the first 10 students who post interesting sample input files. 
Create a README (PDF) file which should have the following information: 
(1) instructions on how to compile the code 
(2) instructions on how to run the code 
(3) justification for the choice of data structures (in terms of time and/or space complexity). 
(4) citations for code referenced online

### Submission 
Upload your assignment as a zipped folder to BrightSpace
In the submission comments provide your github username and hash code [(how?](https://docs.google.com/presentation/d/1TpamPnZ4kqU4pYk86vwq_uqyRJUnHFUXsdNEobfmi7w/edit?usp=sharing)).
Example:  userName123 - 96905470a5a3bc23293ffd5a003350138a1ce8c6
See me during lab for a demo.

## General Requirements 
Separate out code appropriately into methods, one for each purpose. 
You should document your code. The comments should not exceed 72 columns in width. 
Use javadoc style comments if you are coding in Java. Include javadoc style documentation. It is acceptable for this assignment to just have the return type described for each method's documentation. 
All objects, in Java, that may be needed for debugging purposes should  have the "toString()" method defined. By default, just place a toString() in every class. 
Every class that has data members, should have corresponding accessors and mutators (unless the data member(s) is/are for use just within the method.). 
