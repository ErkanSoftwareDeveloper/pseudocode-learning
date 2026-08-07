IF / ELSE

IF / ELSE statements are used to make decisions in a program.

IF → Executes code when a condition is TRUE
ELSE → Executes code when the IF condition is FALSE

Comparison Operators

=  → Equal to
!= → Not equal to
>  → Greater than
<  → Less than
>= → Greater than or equal to
<= → Less than or equal to


# Basic IF
START
  PRINT "Enter your age:"
  INPUT age

  IF age >= 18 THEN
    PRINT "You are an adult."
  END IF
END


# IF / ELSE
START
  PRINT "Enter your age:"
  INPUT age

  IF age >= 18 THEN
    PRINT "You are an adult."
  ELSE
    PRINT "You are a minor."
  END IF
END


# IF / ELSE IF / ELSE
START
  PRINT "Enter your score:"
  INPUT score

  IF score >= 90 THEN
    PRINT "Grade: A"
  ELSE IF score >= 80 THEN
    PRINT "Grade: B"
  ELSE IF score >= 70 THEN
    PRINT "Grade: C"
  ELSE IF score >= 60 THEN
    PRINT "Grade: D"
  ELSE
    PRINT "Grade: F"
  END IF
END


# Check Positive or Negative
START
  PRINT "Enter a number:"
  INPUT number

  IF number > 0 THEN
    PRINT "Positive"
  ELSE IF number < 0 THEN
    PRINT "Negative"
  ELSE
    PRINT "Zero"
  END IF
END


# Check Even or Odd
START
  PRINT "Enter a number:"
  INPUT number

  IF number MOD 2 = 0 THEN
    PRINT "Even"
  ELSE
    PRINT "Odd"
  END IF
END


# Compare Two Numbers
START
  PRINT "Enter first number:"
  INPUT a

  PRINT "Enter second number:"
  INPUT b

  IF a > b THEN
    PRINT "First number is greater."
  ELSE IF a < b THEN
    PRINT "Second number is greater."
  ELSE
    PRINT "Both numbers are equal."
  END IF
END


# Check Password
START
  SET correctPassword TO "12345"

  PRINT "Enter password:"
  INPUT password

  IF password = correctPassword THEN
    PRINT "Access granted."
  ELSE
    PRINT "Access denied."
  END IF
END


# Check Username and Password
START
  SET correctUsername TO "admin"
  SET correctPassword TO "12345"

  PRINT "Enter username:"
  INPUT username

  PRINT "Enter password:"
  INPUT password

  IF username = correctUsername AND password = correctPassword THEN
    PRINT "Login successful."
  ELSE
    PRINT "Invalid username or password."
  END IF
END


# Multiple Conditions
START
  PRINT "Enter your age:"
  INPUT age

  IF age >= 18 AND age <= 65 THEN
    PRINT "You are in the working age range."
  ELSE
    PRINT "You are outside the working age range."
  END IF
END


# OR Condition
START
  PRINT "Enter your day:"
  INPUT day

  IF day = "Saturday" OR day = "Sunday" THEN
    PRINT "It is the weekend."
  ELSE
    PRINT "It is a weekday."
  END IF
END


# Nested IF
START
  PRINT "Enter your age:"
  INPUT age

  IF age >= 18 THEN
    PRINT "You are an adult."

    IF age >= 65 THEN
      PRINT "You are a senior."
    ELSE
      PRINT "You are not a senior."
    END IF

  ELSE
    PRINT "You are a minor."
  END IF
END
