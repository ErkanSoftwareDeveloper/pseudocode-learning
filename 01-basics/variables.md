Variables

Variables are used to store values that can change during a program.

A variable can store different types of values, such as:
- Numbers
- Text
- Boolean values

Common variable operations:
- Declare a variable
- Assign a value
- Change a value
- Use a variable
- Swap variables


# Declare and Assign a Variable
START
  SET age TO 25
  PRINT age
END


# String Variable
START
  SET name TO "Erkan"
  PRINT "Name: " + name
END


# Number Variable
START
  SET age TO 25
  SET height TO 175

  PRINT "Age: " + age
  PRINT "Height: " + height
END


# Boolean Variable
START
  SET isStudent TO TRUE
  PRINT "Is student: " + isStudent
END


# User Input and Variable
START
  PRINT "Enter your name:"
  INPUT name

  PRINT "Hello, " + name
END


# Changing a Variable
START
  SET score TO 10

  PRINT "Score: " + score

  SET score TO 20

  PRINT "New score: " + score
END


# Updating a Variable
START
  SET score TO 10

  SET score TO score + 5

  PRINT "Score: " + score
END


# Increment a Variable
START
  SET counter TO 0

  SET counter TO counter + 1
  SET counter TO counter + 1
  SET counter TO counter + 1

  PRINT "Counter: " + counter
END


# Decrement a Variable
START
  SET lives TO 3

  SET lives TO lives - 1

  PRINT "Lives: " + lives
END


# Variables with Arithmetic
START
  SET a TO 10
  SET b TO 5

  SET sum TO a + b
  SET difference TO a - b
  SET product TO a * b
  SET division TO a / b

  PRINT "Sum: " + sum
  PRINT "Difference: " + difference
  PRINT "Product: " + product
  PRINT "Division: " + division
END


# Copying a Variable
START
  SET original TO 100
  SET copy TO original

  PRINT "Original: " + original
  PRINT "Copy: " + copy
END


# Swapping Two Variables
START
  SET a TO 10
  SET b TO 20

  SET temp TO a
  SET a TO b
  SET b TO temp

  PRINT "A: " + a
  PRINT "B: " + b
END


# Multiple Variables
START
  SET name TO "Erkan"
  SET age TO 25
  SET city TO "Berlin"

  PRINT "Name: " + name
  PRINT "Age: " + age
  PRINT "City: " + city
END


# Variables with User Input
START
  PRINT "Enter your name:"
  INPUT name

  PRINT "Enter your age:"
  INPUT age

  PRINT "Enter your city:"
  INPUT city

  PRINT "Name: " + name
  PRINT "Age: " + age
  PRINT "City: " + city
END


# Variable Reassignment
START
  SET x TO 10

  PRINT "Before: " + x

  SET x TO 50

  PRINT "After: " + x
END
