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

   **Access Object Variables:**

    myobjectx.variable

   **Access Object Functions:**

   myobjectx.function()


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

![d](https://www.researchgate.net/profile/Takaya_Arita/publication/228370446/figure/fig1/AS:669488697602059@1536629952946/Recursive-Thinking-with-a-Theory-of-Mind.png)
