# PROG101_ASSIGNMENT1_MARY_R.M_MAHOI_905006279
Many schools rely on manual attendance registers, which can make attendance monitoring time-consuming and the identification of students with low attendance difficult. This project addresses the need for a more efficient and organized approach to student attendance monitoring in Sierra Leonean schools.

# EDUCATION - A Student Attendance and Academic Alert System
> A Student Attendance and Academic Alert System designed to help schools in Sierra Leone monitor student attendance, calculate attendance percentages, and identify students whose attendance falls below the required 85% threshold.

## Advantages Of The System Selected 
- Saves teachers’ time.
- Reduces calculation errors.
- Identifies students with low attendance.
- Makes attendance monitoring easier.
- Helps improve student attendance.

## Pseudocode Of The Alert System
START
DECLARE studentID daysPresent ,totalDays AS INTEGER
DECLARE attendanceRate ,threshold  AS REAL
DECLARE attendanceStatus , anotherStudent ,studentName AS STRING
SET threshold = 85
SET anotherStudent = "Yes"
WHILE anotherStudent = "Yes"
    DISPLAY “Enter Student ID”
INPUT studentID
DISPLAY “Enter Student Name”
INPUT studentName
DISPLAY “Days Present”
INPUT daysPresent
DISPLAY “Total Days”
    INPUT totalDays

  WHILE 
     totalDays <= 0   OR daysPresent < 0   OR daysPresent > totalDays
     DISPLAY "Invalid attendance information"
        
     DISPLAY “Days Present”
     INPUT daysPresent
     DISPLAY “Total Days”
     INPUT totalDays
  ENDWHILE

SET attendanceRate = (daysPresent / totalDays) * 100
    IF attendanceRate < threshold THEN
        SET attendanceStatus = "Alert"
        DISPLAY attendanceRate & “%”
        DISPLAY "Attendance requires attention"
ELSE
        SET attendanceStatus = "CONGRATULATIONS ON MEETING THE REQUIRED PERCENTAGE"

        DISPLAY attendanceRate & “%”
        DISPLAY "Attendance meets the requirement"
    ENDIF
    DISPLAY attendanceStatus
    INPUT anotherStudent
ENDWHILE
DISPLAY”THANK YOU FOR USING THE STUDENT ATTENDANCE AND ALERT SYSTEM”
STOP

## Flowchart








