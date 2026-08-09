Conditions

Conditions are used to check whether something is TRUE or FALSE.

A condition always produces one of two results:

TRUE
FALSE

Comparison Operators

=  → Equal to
!= → Not equal to
>  → Greater than
<  → Less than
>= → Greater than or equal to
<= → Less than or equal to

Logical Operators

AND → Both conditions must be TRUE
OR  → At least one condition must be TRUE
NOT → Reverses the condition


# Equal To
START
  SET age TO 18

  IF age = 18 THEN
    PRINT "Age is exactly 18."
  END IF
END


# Not Equal To
START
  SET age TO 20

  IF age != 18 THEN
    PRINT "Age is not 18."
  END IF
END


# Greater Than
START
  SET number TO 10

  IF number > 5 THEN
    PRINT "Number is greater than 5."
  END IF
END


# Less Than
START
  SET number TO 3

  IF number < 5 THEN
    PRINT "Number is less than 5."
  END IF
END


# Greater Than or Equal To
START
  SET age TO 18

  IF age >= 18 THEN
    PRINT "You are at least 18."
  END IF
END


# Less Than or Equal To
START
  SET age TO 16

  IF age <= 18 THEN
    PRINT "You are 18 or younger."
  END IF
END


# AND Condition
START
  SET age TO 25
  SET hasID TO TRUE

  IF age >= 18 AND hasID = TRUE THEN
    PRINT "You can enter."
  END IF
END


# OR Condition
START
  SET day TO "Saturday"

  IF day = "Saturday" OR day = "Sunday" THEN
    PRINT "It is the weekend."
  END IF
END


# NOT Condition
START
  SET isRaining TO FALSE

  IF NOT isRaining THEN
    PRINT "You do not need an umbrella."
  END IF
END


# Multiple Conditions
START
  SET age TO 25
  SET hasTicket TO TRUE
  SET isBanned TO FALSE

  IF age >= 18 AND hasTicket = TRUE AND NOT isBanned THEN
    PRINT "You can enter."
  ELSE
    PRINT "You cannot enter."
  END IF
END


# Boolean Variable as a Condition
START
  SET isLoggedIn TO TRUE

  IF isLoggedIn THEN
    PRINT "Welcome back."
  ELSE
    PRINT "Please log in."
  END IF
END


# Check a Range
START
  PRINT "Enter a number:"
  INPUT number

  IF number >= 1 AND number <= 100 THEN
    PRINT "Number is between 1 and 100."
  ELSE
    PRINT "Number is outside the range."
  END IF
END


# Compare Two Values
START
  PRINT "Enter first number:"
  INPUT a

  PRINT "Enter second number:"
  INPUT b

  IF a = b THEN
    PRINT "The numbers are equal."
  ELSE IF a > b THEN
    PRINT "The first number is greater."
  ELSE
    PRINT "The second number is greater."
  END IF
END


# Multiple Boolean Conditions
START
  SET hasMoney TO TRUE
  SET storeOpen TO TRUE
  SET productAvailable TO TRUE

  IF hasMoney AND storeOpen AND productAvailable THEN
    PRINT "You can buy the product."
  ELSE
    PRINT "You cannot buy the product."
  END IF
END
