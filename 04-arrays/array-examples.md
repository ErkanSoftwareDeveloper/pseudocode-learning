Arrays

An array is a collection of multiple values stored in a single variable.

Arrays can contain multiple values of the same type.

Each value in an array has an index.

In most programming languages, the first index is 0.


# Create an Array
START
  SET fruits TO ["Apple", "Banana", "Orange"]

  PRINT fruits
END


# Access an Array Element
START
  SET fruits TO ["Apple", "Banana", "Orange"]

  PRINT fruits[0]
  PRINT fruits[1]
  PRINT fruits[2]
END


# Change an Array Element
START
  SET fruits TO ["Apple", "Banana", "Orange"]

  SET fruits[1] TO "Mango"

  PRINT fruits
END


# Array Length
START
  SET numbers TO [10, 20, 30, 40, 50]

  SET length TO LENGTH(numbers)

  PRINT "Array length: " + length
END


# Loop Through an Array
START
  SET fruits TO ["Apple", "Banana", "Orange", "Mango"]

  FOR each fruit IN fruits
    PRINT fruit
  END FOR
END


# Loop Through an Array Using Index
START
  SET numbers TO [10, 20, 30, 40, 50]

  FOR i FROM 0 TO LENGTH(numbers) - 1
    PRINT numbers[i]
  END FOR
END


# Sum Array Values
START
  SET numbers TO [10, 20, 30, 40, 50]
  SET sum TO 0

  FOR each number IN numbers
    SET sum TO sum + number
  END FOR

  PRINT "Sum: " + sum
END


# Find the Largest Number
START
  SET numbers TO [10, 25, 7, 42, 18]

  SET largest TO numbers[0]

  FOR each number IN numbers

    IF number > largest THEN
      SET largest TO number
    END IF

  END FOR

  PRINT "Largest number: " + largest
END


# Find the Smallest Number
START
  SET numbers TO [10, 25, 7, 42, 18]

  SET smallest TO numbers[0]

  FOR each number IN numbers

    IF number < smallest THEN
      SET smallest TO number
    END IF

  END FOR

  PRINT "Smallest number: " + smallest
END


# Search for a Value
START
  SET numbers TO [10, 20, 30, 40, 50]

  PRINT "Enter a number to search:"
  INPUT target

  SET found TO FALSE

  FOR each number IN numbers

    IF number = target THEN
      SET found TO TRUE
    END IF

  END FOR

  IF found = TRUE THEN
    PRINT "Number found."
  ELSE
    PRINT "Number not found."
  END IF
END


# Count a Specific Value
START
  SET numbers TO [5, 10, 5, 20, 5, 30]
  SET target TO 5
  SET count TO 0

  FOR each number IN numbers

    IF number = target THEN
      SET count TO count + 1
    END IF

  END FOR

  PRINT "Number appears " + count + " times."
END


# Calculate the Average
START
  SET numbers TO [10, 20, 30, 40, 50]
  SET sum TO 0

  FOR each number IN numbers
    SET sum TO sum + number
  END FOR

  SET average TO sum / LENGTH(numbers)

  PRINT "Average: " + average
END


# Reverse an Array
START
  SET numbers TO [1, 2, 3, 4, 5]

  FOR i FROM LENGTH(numbers) - 1 TO 0 STEP -1
    PRINT numbers[i]
  END FOR
END


# Array with User Input
START
  SET numbers TO []

  FOR i FROM 1 TO 5
    PRINT "Enter number:"
    INPUT number

    ADD number TO numbers
  END FOR

  PRINT "Numbers:"
  PRINT numbers
END


# Remove an Element
START
  SET fruits TO ["Apple", "Banana", "Orange", "Mango"]

  REMOVE fruits[1]

  PRINT fruits
END


# Add an Element
START
  SET fruits TO ["Apple", "Banana", "Orange"]

  ADD "Mango" TO fruits

  PRINT fruits
END


# Two Arrays
START
  SET names TO ["Erkan", "Ali", "Mehmet"]
  SET ages TO [25, 30, 22]

  FOR i FROM 0 TO LENGTH(names) - 1
    PRINT names[i] + " is " + ages[i] + " years old."
  END FOR
END


# Nested Arrays
START
  SET matrix TO [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
  ]

  PRINT matrix[0][0]
  PRINT matrix[1][1]
  PRINT matrix[2][2]
END
