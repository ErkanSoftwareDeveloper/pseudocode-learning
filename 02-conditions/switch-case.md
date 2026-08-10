Switch / Case

A switch-case statement is used to compare one value
against multiple possible values.

SWITCH → Starts the selection
CASE → Checks a possible value
DEFAULT → Runs when no case matches
BREAK → Stops the switch after a matching case


# Basic Switch-Case
START
  PRINT "Enter a number from 1 to 3:"
  INPUT number

  SWITCH number

    CASE 1:
      PRINT "You selected one."
      BREAK

    CASE 2:
      PRINT "You selected two."
      BREAK

    CASE 3:
      PRINT "You selected three."
      BREAK

    DEFAULT:
      PRINT "Invalid number."

  END SWITCH
END


# Switch-Case with Text
START
  PRINT "Enter a day:"
  INPUT day

  SWITCH day

    CASE "Monday":
      PRINT "Start of the week."
      BREAK

    CASE "Friday":
      PRINT "Almost the weekend."
      BREAK

    CASE "Saturday":
      PRINT "It is the weekend."
      BREAK

    CASE "Sunday":
      PRINT "It is the weekend."
      BREAK

    DEFAULT:
      PRINT "It is a weekday."

  END SWITCH
END


# Switch-Case with Multiple Cases
START
  PRINT "Enter a month:"
  INPUT month

  SWITCH month

    CASE 1:
    CASE 2:
    CASE 12:
      PRINT "Winter."
      BREAK

    CASE 3:
    CASE 4:
    CASE 5:
      PRINT "Spring."
      BREAK

    CASE 6:
    CASE 7:
    CASE 8:
      PRINT "Summer."
      BREAK

    CASE 9:
    CASE 10:
    CASE 11:
      PRINT "Autumn."
      BREAK

    DEFAULT:
      PRINT "Invalid month."

  END SWITCH
END


# Simple Calculator
START
  PRINT "Enter first number:"
  INPUT a

  PRINT "Enter second number:"
  INPUT b

  PRINT "Enter operator (+, -, *, /):"
  INPUT operator

  SWITCH operator

    CASE "+":
      SET result TO a + b
      PRINT "Result: " + result
      BREAK

    CASE "-":
      SET result TO a - b
      PRINT "Result: " + result
      BREAK

    CASE "*":
      SET result TO a * b
      PRINT "Result: " + result
      BREAK

    CASE "/":
      IF b != 0 THEN
        SET result TO a / b
        PRINT "Result: " + result
      ELSE
        PRINT "Cannot divide by zero."
      END IF
      BREAK

    DEFAULT:
      PRINT "Invalid operator."

  END SWITCH
END


# Menu Selection
START
  PRINT "1. Start Game"
  PRINT "2. Load Game"
  PRINT "3. Settings"
  PRINT "4. Exit"

  PRINT "Choose an option:"
  INPUT choice

  SWITCH choice

    CASE 1:
      PRINT "Starting game..."
      BREAK

    CASE 2:
      PRINT "Loading game..."
      BREAK

    CASE 3:
      PRINT "Opening settings..."
      BREAK

    CASE 4:
      PRINT "Goodbye!"
      BREAK

    DEFAULT:
      PRINT "Invalid option."

  END SWITCH
END


# Switch-Case with a Variable
START
  SET role TO "admin"

  SWITCH role

    CASE "admin":
      PRINT "Full access granted."
      BREAK

    CASE "editor":
      PRINT "Edit access granted."
      BREAK

    CASE "user":
      PRINT "Limited access granted."
      BREAK

    DEFAULT:
      PRINT "Unknown role."

  END SWITCH
END


# Switch-Case vs IF / ELSE
START
  PRINT "Enter a number:"
  INPUT number

  SWITCH number

    CASE 1:
      PRINT "One."
      BREAK

    CASE 2:
      PRINT "Two."
      BREAK

    CASE 3:
      PRINT "Three."
      BREAK

    DEFAULT:
      PRINT "Other number."

  END SWITCH
END
