For Loops

A for loop is used to repeat a block of code
a specific number of times.

A for loop usually has:
- A starting value
- An ending condition
- A step


# Basic For Loop
START
  FOR i FROM 1 TO 5
    PRINT i
  END FOR
END


# Count from 0 to 5
START
  FOR i FROM 0 TO 5
    PRINT i
  END FOR
END


# Count from 1 to 10
START
  FOR i FROM 1 TO 10
    PRINT i
  END FOR
END


# Count with a Step
START
  FOR i FROM 0 TO 10 STEP 2
    PRINT i
  END FOR
END


# Count Backwards
START
  FOR i FROM 10 TO 1 STEP -1
    PRINT i
  END FOR
END


# Print a Message Multiple Times
START
  FOR i FROM 1 TO 5
    PRINT "Hello!"
  END FOR
END


# Calculate a Sum
START
  SET sum TO 0

  FOR i FROM 1 TO 10
    SET sum TO sum + i
  END FOR

  PRINT "Sum: " + sum
END


# Multiplication Table
START
  PRINT "Enter a number:"
  INPUT number

  FOR i FROM 1 TO 10
    SET result TO number * i
    PRINT number + " x " + i + " = " + result
  END FOR
END


# Loop with an IF Condition
START
  FOR i FROM 1 TO 10

    IF i MOD 2 = 0 THEN
      PRINT i + " is even."
    END IF

  END FOR
END


# Print Odd Numbers
START
  FOR i FROM 1 TO 20

    IF i MOD 2 != 0 THEN
      PRINT i
    END IF

  END FOR
END


# Find Numbers Greater Than 5
START
  FOR i FROM 1 TO 10

    IF i > 5 THEN
      PRINT i
    END IF

  END FOR
END


# For Loop with User Input
START
  PRINT "How many times should the message be printed?"
  INPUT count

  FOR i FROM 1 TO count
    PRINT "Hello!"
  END FOR
END


# Factorial
START
  PRINT "Enter a number:"
  INPUT number

  SET result TO 1

  FOR i FROM 1 TO number
    SET result TO result * i
  END FOR

  PRINT "Factorial: " + result
END


# Nested For Loops
START
  FOR i FROM 1 TO 3

    FOR j FROM 1 TO 3
      PRINT "i: " + i + ", j: " + j
    END FOR

  END FOR
END


# Nested Loop - Multiplication Tables
START
  FOR i FROM 1 TO 10

    FOR j FROM 1 TO 10
      SET result TO i * j
      PRINT i + " x " + j + " = " + result
    END FOR

  END FOR
END


# Loop Through a List
START
  SET fruits TO ["Apple", "Banana", "Orange", "Mango"]

  FOR each fruit IN fruits
    PRINT fruit
  END FOR
END


# Find a Specific Value
START
  SET numbers TO [10, 20, 30, 40, 50]
  SET target TO 30

  FOR each number IN numbers

    IF number = target THEN
      PRINT "Number found."
    END IF

  END FOR
END


# Count Values in a List
START
  SET numbers TO [5, 10, 15, 20, 25]
  SET count TO 0

  FOR each number IN numbers

    IF number >= 10 THEN
      SET count TO count + 1
    END IF

  END FOR

  PRINT "Numbers greater than or equal to 10: " + count
END
