# Student Grade Database Analysis
In this project, we will be working with a database of course records from a (fictional) university called Syntheticus University, which was founded in Fall 2000. The university offers six undergraduate degree programs: Biology, Chemistry, Computer Science, Mathematics, and Physics. The data we will work with is assumed to have been collected immediately after the end of the Spring 2021 term.  

**Below is the list of the files and their description:**  

 **accepted.csv** - Contains a single record for any student that has been accepted into IU, whether or not they actually enrolled in courses.  
 - acc_term_id – The term for which the student was accepted to enroll. This is a string consisting of the year followed by 'A' for Spring and 'B' for Fall. Note than not all accepted students do enroll.
 - sid – Student ID Number. Represented as an integer.  
 - first_name – A string representing the student's first name.  
 - last_name – A string representing the student's last name.       
 - major – A string representing the student's major. ('BIO', 'CHM', 'CSC', 'MTH', or 'PHY')  

**alumni.csv** – Contains a column of sid numbers for students who have graduated from SU.
 - expelled.csv – Contains a column of sid numbers for students who have been expelled from SU.  
 - unretained.csv – Contains a column of sid numbers for students who have transferred from SU.   
 
**faculty.csv** – Contains information for every faculty member who ever has taught at SU.
  - fid – Faculty ID Number. Represented as an integer.  
  - first_name – A string representing the faculty member's first name.  
  - last_name – A string representing the faculty member's last name.  
  - dept – The dept the faculty member teaches in. ('BIO', 'CHM', 'CSC', 'MTH', 'PHY', or 'GEN')   
   
**courses.csv** – Contains information for all courses offered by IU.  
  - dept – The dept that the course is offered in. ('BIO', 'CHM', 'CSC', 'MTH', 'PHY', or 'GEN')  
  - course – This is a string containing the prefix and number of the course.  
  - prereq – A string indicating the prerequisite for the course.  
  - credits – An integer representing the number of credit hours for the course.  
  
 **grades.csv** – This file contains grade records. Each record represents a grade given to a particular student in a particular course. There is one record for every grade that has every been assigned in a class at SU. This is the largest file in the database.  
  - term_id – The term during which the grade was earned. This is a string consisting of the year followed by 'A' for Spring and 'B' for Fall.  
  - course – A string representing the prefix and number of the course.  
  - sid – An integer representing the SID for the student earning the grade.  
  - fid – An integer representing the Faculty ID number for the course instructor.  
  - grade – A string representing the letter grade that was assigned. ('A', 'B', 'C', 'D', or 'F')

**Please take note the following comments relating to this dataset.**
- Not all accepted students actually attend the university. If an accepted student did enroll in courses, then they will have at least one grade record in the grades.csv file.
- We assume that students are not able to withdraw from courses or receive incomplete grades.
- There are only three possible outcomes for a student who enrolls at the university: They graduate, they decide to leave the university (and are thus unretained), or they are expelled.
- For simplicity, we assume that students do not double major, and that no student changes their major.
- The convention we have adopted of using A to denote Spring terms and B to denote Fall terms is used simply to ensure that the terms appear in the correct chronological order when sorted.


