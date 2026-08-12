While Loops

A while loop repeats a block of code as long as a condition is TRUE.

A while loop usually has:
- A condition
- A block of code
- A way to change the condition


# Basic While Loop
START
  SET counter TO 1

  WHILE counter <= 5
    PRINT counter
    SET counter TO counter + 1
  END WHILE
END


# Count from 1 to 10
START
  SET number TO 1

  WHILE number <= 10
    PRINT number
    SET number TO number + 1
  END WHILE
END


# Count Backwards
START
  SET number TO 10

  WHILE number >= 1
    PRINT number
    SET number TO number - 1
  END WHILE
END


# Print a Message
START
  SET counter TO 1

  WHILE counter <= 5
    PRINT "Hello!"
    SET counter TO counter + 1
  END WHILE
END


# Sum of Numbers
START
  SET number TO 1
  SET sum TO 0

  WHILE number <= 10
    SET sum TO sum + number
    SET number TO number + 1
  END WHILE

  PRINT "Sum: " + sum
END


# Even Numbers
START
  SET number TO 2

  WHILE number <= 20
    PRINT number
    SET number TO number + 2
  END WHILE
END


# While Loop with User Input
START
  PRINT "Enter a number greater than 0:"
  INPUT number

  WHILE number <= 0
    PRINT "Invalid number. Try again:"
    INPUT number
  END WHILE

  PRINT "Valid number: " + number
END


# Password Validation
START
  SET correctPassword TO "12345"

  PRINT "Enter password:"
  INPUT password

  WHILE password != correctPassword
    PRINT "Incorrect password. Try again:"
    INPUT password
  END WHILE

  PRINT "Access granted."
END


# Countdown
START
  PRINT "Enter a starting number:"
  INPUT number

  WHILE number >= 0
    PRINT number
    SET number TO number - 1
  END WHILE

  PRINT "Countdown finished!"
END


# Factorial
START
  PRINT "Enter a number:"
  INPUT number

  SET result TO 1
  SET counter TO 1

  WHILE counter <= number
    SET result TO result * counter
    SET counter TO counter + 1
  END WHILE

  PRINT "Factorial: " + result
END


# Find a Number
START
  SET target TO 7
  SET number TO 0

  WHILE number != target
    PRINT "Enter a number:"
    INPUT number
  END WHILE

  PRINT "Correct number!"
END


# While Loop with IF
START
  SET number TO 1

  WHILE number <= 10

    IF number MOD 2 = 0 THEN
      PRINT number + " is even."
    ELSE
      PRINT number + " is odd."
    END IF

    SET number TO number + 1

  END WHILE
END


# Menu Loop
START
  SET choice TO 0

  WHILE choice != 4
    PRINT "1. Start"
    PRINT "2. Settings"
    PRINT "3. Help"
    PRINT "4. Exit"

    PRINT "Choose an option:"
    INPUT choice

    IF choice = 1 THEN
      PRINT "Starting..."
    ELSE IF choice = 2 THEN
      PRINT "Opening settings..."
    ELSE IF choice = 3 THEN
      PRINT "Opening help..."
    ELSE IF choice = 4 THEN
      PRINT "Goodbye!"
    ELSE
      PRINT "Invalid option."
    END IF

  END WHILE
END


# Infinite Loop
START
  WHILE TRUE
    PRINT "This loop runs forever."
  END WHILE
END
