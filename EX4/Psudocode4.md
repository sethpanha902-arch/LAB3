START

INPUT numberOfStudents

FOR each student

    INPUT student name
    INPUT student ID

    FOR 5 subjects
        INPUT subject score
    END FOR

    CREATE Student object

    CALCULATE total marks
    CALCULATE average

END FOR

FOR each student

    DISPLAY student name and ID
    DISPLAY 5 subject scores
    DISPLAY total marks
    DISPLAY average

    IF average >= 90
        DISPLAY Grade A
    ELSE IF average >= 75
        DISPLAY Grade B
    ELSE IF average >= 50
        DISPLAY Grade C
    ELSE
        DISPLAY Grade F
    END IF

END FOR

CLOSE Scanner

END
