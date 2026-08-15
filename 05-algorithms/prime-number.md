Prime Numbers

A prime number is a number greater than 1
that has exactly two factors:

- 1
- Itself

Examples of prime numbers:

2, 3, 5, 7, 11, 13, 17, 19

Examples of non-prime numbers:

4, 6, 8, 9, 10, 12


# Check if a Number is Prime
START
  PRINT "Enter a number:"
  INPUT number

  SET isPrime TO TRUE

  IF number <= 1 THEN
    SET isPrime TO FALSE
  END IF

  FOR i FROM 2 TO number - 1

    IF number MOD i = 0 THEN
      SET isPrime TO FALSE
    END IF

  END FOR

  IF isPrime THEN
    PRINT number + " is a prime number."
  ELSE
    PRINT number + " is not a prime number."
  END IF
END


# Check if 7 is Prime
START
  SET number TO 7
  SET isPrime TO TRUE

  FOR i FROM 2 TO number - 1

    IF number MOD i = 0 THEN
      SET isPrime TO FALSE
    END IF

  END FOR

  IF isPrime THEN
    PRINT "7 is prime."
  ELSE
    PRINT "7 is not prime."
  END IF
END


# Check Multiple Numbers
START
  FOR number FROM 2 TO 10

    SET isPrime TO TRUE

    FOR i FROM 2 TO number - 1

      IF number MOD i = 0 THEN
        SET isPrime TO FALSE
      END IF

    END FOR

    IF isPrime THEN
      PRINT number
    END IF

  END FOR
END


# Count Prime Numbers
START
  PRINT "Enter a limit:"
  INPUT limit

  SET count TO 0

  FOR number FROM 2 TO limit

    SET isPrime TO TRUE

    FOR i FROM 2 TO number - 1

      IF number MOD i = 0 THEN
        SET isPrime TO FALSE
      END IF

    END FOR

    IF isPrime THEN
      SET count TO count + 1
    END IF

  END FOR

  PRINT "Prime numbers found: " + count
END


# Print Prime Numbers Up To N
START
  PRINT "Enter a limit:"
  INPUT limit

  FOR number FROM 2 TO limit

    SET isPrime TO TRUE

    FOR i FROM 2 TO number - 1

      IF number MOD i = 0 THEN
        SET isPrime TO FALSE
      END IF

    END FOR

    IF isPrime THEN
      PRINT number
    END IF

  END FOR
END


# Optimized Prime Check
START
  PRINT "Enter a number:"
  INPUT number

  SET isPrime TO TRUE

  IF number <= 1 THEN
    SET isPrime TO FALSE
  END IF

  FOR i FROM 2 TO SQRT(number)

    IF number MOD i = 0 THEN
      SET isPrime TO FALSE
    END IF

  END FOR

  IF isPrime THEN
    PRINT number + " is prime."
  ELSE
    PRINT number + " is not prime."
  END IF
END


# Find the First Prime Number Greater Than N
START
  PRINT "Enter a number:"
  INPUT number

  SET current TO number + 1

  WHILE TRUE

    SET isPrime TO TRUE

    FOR i FROM 2 TO current - 1

      IF current MOD i = 0 THEN
        SET isPrime TO FALSE
      END IF

    END FOR

    IF isPrime THEN
      PRINT "Next prime: " + current
      BREAK
    END IF

    SET current TO current + 1

  END WHILE
END


# Prime Numbers in an Array
START
  SET numbers TO [2, 4, 5, 8, 11, 15, 17]

  FOR each number IN numbers

    SET isPrime TO TRUE

    IF number <= 1 THEN
      SET isPrime TO FALSE
    END IF

    FOR i FROM 2 TO number - 1

      IF number MOD i = 0 THEN
        SET isPrime TO FALSE
      END IF

    END FOR

    IF isPrime THEN
      PRINT number
    END IF

  END FOR
END
