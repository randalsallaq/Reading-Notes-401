# Classes and Objects

  * Objects get their variables and functions from classes.
  * Classes are essentially a template to create your objects.

  * Accessing Object Variables
  
  
  ```
  class MyClass:
      variable = "blah"
  
      def function(self):
          print("This is a message inside the class.")

  myobjectx = MyClass()
  
  myobjectx.variable
  ```

   ***Accessing Object Variables:***

   we can di it using myobjectx.variable

   ***Accessing Object Functions:***

   we can do it using myobjectx.function()


   ## Thinking recursively in python
   
   If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.

   in python, a recursive function is a function that calls itself and repeats its behavior until some conditions are met to return a result all recursive functions share the same structure, a base case, and a recursive case

   Recursive function for calculating n! implemented in Python:
   ```
    def factorial_recursive(n):
    # Base case: 1! = 1
    if n == 1:
        return 1

    # Recursive case: n! = n * (n-1)!
    else:
        return n * factorial_recursive(n-1)
   ``
