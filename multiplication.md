# Multiplication

Scenario: Multiplication of two positive integer numbers
  
  Given the calculator is on and the calculator screen is clear.

  When I type in positive number\
        And press multiply\
        And type in positive number\
        And press equals.
  
  Then the calculator screen will show multiplication of two positive numbers.

Scenario: Multiplication of two negative numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in negative number\
        And press multiply\
        And press opening bracket\
        And type in negative number\
        And press closing bracket\
        And press equals.
  
  Then the calculator screen will show multiplication of two negative numbers.
  
Scenario: Multiplication of one positive and one negative numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in positive number\
        And press multiply\
        And press opening bracket\
        And type in negative number\
        And press closing bracket\
        And press equals.
  
  Then the calculator screen will show multiplication of two numbers.
  
Scenario: Multiplication of more than two numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in number\
        And press multiply\
        And type in another number\
        And press multiply\
        And type in another number\
        And repeat press multiply and type in another number for remaining numbers\
        And press equals.
  
  Then the calculator screen will show multiplication of all the numbers.

Scenario: Multiplication of two decimal numbers.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in decimal number\
        And press multiply\
        And type in decimal number\
        And press equals.
  
  Then the calculator screen will show multiplication of two decimal numbers.
  
Scenario: When input syntax is invalid.
  
  Given the calculator is on and the calculator screen is clear.

  When I type in number\
  And press multiply\
        And type in number\
        And press multiply\
        And press equals.
  
  Then the calculator will show invalid syntax on calculator screen.

Scenario: multiplication of two fractions.
  
  Given the calculator is on and the calculator screen is clear.

  When I press opening bracket\
	And type in fraction\
        And closing bracket\
        And press multiply\
        And press opening bracket\
        And type in fraction\
        And closing bracket\
        And press equals.
  
  Then the calculator screen will show multiplication of fractions.
  
Scenario: Multiplication of numbers where result goes out of range.

  Given the calculator is on and the calculator screen is clear.

  When I type in number\ 
	And press multiply\
	And type in number\
	And press equals.

  Then the calculator will show out of range on calculator screen.

Scenarios: Pressing multiply button multiple times.

  Given the calculator is on and the calculator screen is clear.

  When I type in number\ 
	And press multiply\
	And press multiply again\
	And type in number\
	And press equals.

  Then the calculator will simply show multiplication on calculator screen.
  
Scenarios: Multiplication by one.

  Given the calculator is on and the calculator screen is clear.

  When I type in first number\ 
	And press multiply\
	And type in 1\
	And press equals.

  Then the calculator will show the first number on calculator screen.
  
Scenarios: Multiplication by zero.

  Given the calculator is on and the calculator screen is clear.

  When I type in first number\ 
	And press multiply\
	And type in 0\
	And press equals.

  Then the calculator will show zero on calculator screen.
