Factorial

The factorial of a positive integer is the product of that number
and all positive integers smaller than it.

The factorial of n is written as:

n!

For example:

5! = 5 × 4 × 3 × 2 × 1
5! = 120

By definition:

0! = 1


# Basic Factorial
START
  PRINT "Enter a number:"
  INPUT number

  SET result TO 1

  FOR i FROM 1 TO number
    SET result TO result * i
  END FOR

  PRINT "Factorial: " + result
END


# Factorial Using While Loop
START
  PRINT "Enter a number:"
  INPUT number

  SET result TO 1
  SET i TO 1

  WHILE i <= number
    SET result TO result * i
    SET i TO i + 1
  END WHILE

  PRINT "Factorial: " + result
END


# Factorial of 5
START
  SET number TO 5
  SET result TO 1

  FOR i FROM 1 TO number
    SET result TO result * i
  END FOR

  PRINT "5! = " + result
END


# Factorial with Step-by-Step Output
START
  PRINT "Enter a number:"
  INPUT number

  SET result TO 1

  FOR i FROM 1 TO number
    SET result TO result * i
    PRINT "Step " + i + ": " + result
  END FOR

  PRINT "Final result: " + result
END


# Check for Zero
START
  PRINT "Enter a number:"
  INPUT number

  IF number = 0 THEN
    PRINT "0! = 1"
  ELSE
    SET result TO 1

    FOR i FROM 1 TO number
      SET result TO result * i
    END FOR

    PRINT number + "! = " + result
  END IF
END


# Check for Negative Numbers
START
  PRINT "Enter a number:"
  INPUT number

  IF number < 0 THEN
    PRINT "Factorial is not defined for negative numbers."
  ELSE
    SET result TO 1

    FOR i FROM 1 TO number
      SET result TO result * i
    END FOR

    PRINT number + "! = " + result
  END IF
END


# Factorial Using a Function
FUNCTION factorial(number)

  SET result TO 1

  FOR i FROM 1 TO number
    SET result TO result * i
  END FOR

  RETURN result

END FUNCTION


START
  PRINT "Enter a number:"
  INPUT number

  SET result TO factorial(number)

  PRINT "Factorial: " + result
END


# Recursive Factorial
FUNCTION factorial(number)

  IF number = 0 THEN
    RETURN 1
  ELSE
    RETURN number * factorial(number - 1)
  END IF

END FUNCTION


START
  PRINT "Enter a number:"
  INPUT number

  SET result TO factorial(number)

  PRINT "Factorial: " + result
END
