## Ques1. What is the difference between '==' and 'is' operators in Python? Provide an example for each.
### '==' is used to check equality conditions or for doing comparisons. for example 1 == 2 - checks whether 1 is equal to 2 or not? so basically it will return false as 1 is not equal to 2. 
### '=' is used to assign purpose. i.e. assigning values to some variable. for example, name = 'vishal' . This will basically assign 'vishal' to variable called name.

## Ques2. Explain the concept of mutability of objects in Python with suitable examples.
### Mutability in python means once object is created it can be further modified, updated or altered. for example, array or list in python.
### Immutability in python means once object is created you cannot further modify, update or alter anything to it. for example, strings in python.

## Ques3. How is a ternary conditional operator used in Python? Provide an example.
### ternary operator determines if a condition is true or false and then returns the appropriate value in accordance with the result. for example
#### a, b = 2, 5
#### print(a if a < b else b)

## Ques4. What is the purpose of the 'pass' statement in Python? Provide a code example.
### 'pass' statement used as a placeholder when syntactically, a statement is required, but you don't want to execute/write any code.for example
#### def myfun():
####    pass

## Ques5. What are the different logical operators available in Python? Provide examples for each.
### and: Returns True if both operands are true, otherwise, it returns False.
#### print(True and True) output: True
#### print(True and False) output: False
### or: Returns True if at least one of the operands is true, otherwise, it returns False.
#### print(True or True) output: True
#### print(True or False) output: True
### not: Returns the opposite boolean value of the operand.
#### print(not True) output: False
#### print(not False) output: True


## Ques6. Explain the difference between 'and' and '&' operators in Python with examples.
### 'and' is used for logical conjunction. example 
#### x = 5
#### y = 10
#### z = 15
#### if x < y and y < z:
####     print("Both conditions are true")
#### else:
####     print("At least one condition is false")
### while '&' is used for performing bitwise AND operation on integers. for example
#### x = 5
#### y = 3 
#### result = x & y  # binary representation: 0001 (1 in decimal)
#### print("Bitwise AND result:", result)


## Ques7. What is the 'in' keyword used for in Python? Provide an example.
### In Python, the in keyword is used to check for membership within a sequence
#### sentence = "The quick brown fox jumps over the lazy dog"
#### if 'fox' in sentence:
####     print("Yes, 'fox' is in the string")
#### else:
####     print("No, 'fox' is not in the string")

## Ques8. What are the different comparison operators in Python? Provide examples for each.
### == (Equal to): Checks if two values are equal.
#### result = 1 == 2  
#### print(result) output: False

### != (Not equal to): Checks if two values are not equal.
#### result = 1 != 2 
#### print(result) output: True

### > (Greater than): Checks if the left operand is greater than the right operand.
#### result = 1 > 2
#### print(result) output: False

### < (Less than): Checks if the left operand is less than the right operand.
#### result = 1 < 2
#### print(result) output: True

### >= (Greater than or equal to): Checks if the left operand is greater than or equal to the right operand.
#### result = 1 >= 2
#### print(result) output: False

### <= (Less than or equal to): Checks if the left operand is less than or equal to the right operand.
#### result = 1 <= 2
#### print(result) output: True

## Ques9. How does the 'not' operator work in Python? Provide an example.
### In Python, the not operator is a unary operator used to negate the value of a boolean expression. It returns True if the expression is False, and False if the expression is True. for example
#### print(not True) output: False
#### print(not False) output: True
## Ques10. Explain the concept of short-circuit evaluation in Python with an example.
### Short-circuit evaluation is a concept used in programming languages, including Python, where the evaluation of an expression stops as soon as the result is known with certainty, without evaluating the remaining parts of the expression.
###  the 'and' and 'or' operators use short-circuit evaluation
### for example i have a function
#### def func():
#### print("This function is called")
####    return True
#### result1 = False and func() #here function will not be called because of the False at starting in case of 'and'
#### result2 = True or func() #here function will not be called because of the True at starting in case of 'or'