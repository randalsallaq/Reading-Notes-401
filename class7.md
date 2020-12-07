# Python Scope

#### The scope of a variable refers to the places that you can see or access a variable.

![s](https://media.geeksforgeeks.org/wp-content/uploads/types_namespace-1.png)


There is two general scopes:

- ***Global scope***: The names that you define in this scope are available to all your code.

- ***Local scope***: The names that you define in this scope are only available or visible to the code within the scope.


# What id LEGB

### LEGB stands for Local, Enclosing, Global, Built-in.
The order Local, Enclosing, Global, Built-in is the order of precedence for scope resolution. That means Python searches for the value of a name in each of these namespaces in turn.

![v](https://sebastianraschka.com/images/blog/2014/scope_resolution_legb_rule/scope_resolution_1.png)


- ***Local (or function) scope***: The local scope is the scope of all objects in the current namespace.
- ***Enclosing (or nonlocal) scope***: The enclosing scope is the scope of any objects in the namespace that encloses the current namespace, which may or may not exist. 
- ***Global (or module) scope***: The global scope is the scope of objects in the module-level namespace. Creating a variable outside of a function or class will put it in the global namespace.
- ***Built-in scope***: The built-in scope is the scope of all objects that are built into the Python language. Reserved names like dict are found in this namespace.



**class6 references**

- [Python Scope](https://realpython.com/python-scope-legb-rule/#names-and-scopes-in-python)
- [Don’t be CONFUSED by BIG O notation anymore!](https://www.youtube.com/watch?v=5Uqawfl0VHQ)
- [Rolling Dice Examples](https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Program_Example_1_3)
