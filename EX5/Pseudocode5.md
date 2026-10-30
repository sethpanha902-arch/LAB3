START

INPUT number of customers

FOR each customer
    INPUT account number

    WHILE account number is not 14 digits
        DISPLAY invalid account number
        INPUT account number again
    END WHILE

    INPUT customer name
    INPUT initial balance

    CREATE Account object
    ADD account to account list
END FOR

DO
    DISPLAY banking menu
    INPUT choice

    IF choice = 1 OR choice = 2 THEN

        INPUT account number
        SEARCH for account

        IF account not found THEN
            DISPLAY "Account not found"

        ELSE
            INPUT amount

            IF choice = 1 THEN
                DEPOSIT amount
            ELSE
                WITHDRAW amount
                IF amount > balance THEN
                    DISPLAY "Insufficient balance"
                END IF
            END IF

            DISPLAY updated account details
        END IF

    ELSE IF choice = 3 THEN
        DISPLAY all accounts
    END IF

WHILE choice != 0

DISPLAY thank you message
CLOSE Scanner

END
