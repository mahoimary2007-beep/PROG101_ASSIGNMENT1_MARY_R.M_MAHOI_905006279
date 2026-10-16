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
<img width="1280" height="1253" alt="WhatsApp Image 2026-10-15 at 13 56 19" src="https://github.com/user-attachments/assets/c41277f7-e89f-4e70-a184-b66cddb6ba27" />
<img width="960" height="915" alt="WhatsApp Image 2026-10-15 at 13 56 15" src="https://github.com/user-attachments/assets/f3d71f1a-aa54-4fac-944c-2c39f310556d" />
<img width="822" height="942" alt="WhatsApp Image 2026-10-15 at 13 56 16" src="https://github.com/user-attachments/assets/6ebc64c4-eb18-442d-b509-bc900f288c84" />
<img width="1280" height="1038" alt="WhatsApp Image 2026-10-15 at 13 56 20" src="https://github.com/user-attachments/assets/51dfe1bf-e684-4d05-a08c-83f4244bacae" />
<img width="1280" height="998" alt="WhatsApp Image 2026-10-15 at 13 56 26" src="https://github.com/user-attachments/assets/78d29a63-dec2-4f2e-87e3-1fcfeb1a3a7a" />




















