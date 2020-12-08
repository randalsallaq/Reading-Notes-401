# List comprehension
 ### List comprehension is an elegant way to define and create lists based on existing lists. List comprehension is generally more compact and faster than normal functions and loops for creating list. However, we should avoid writing very long list comprehensions in one line to ensure that code is user-friendly.
 
 ![l](https://www.mrdbourke.com/content/images/2019/09/python-list-comprehension-article.png)
 
 If you used to do it like this:
```
new_list = []
for i in old_list:
    if filter(i):
        new_list.append(expressions(i))

```
You can obtain the same thing using list comprehension:
```
new_list = [expression(i) for i in old_list if filter(i)]

```

#### List Comprehension as an Alternative

List comprehension is a complete substitute to for loops, lambda function as well as the functions map(), filter() and reduce(). What's more, for some people, list comprehension can even be easier to understand and use in practice

![f](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQul4QWlJefwnB0rpuiTRrlXmdR5cQIUkM4TQ&usqp=CAU)

## ***references:***
[List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)
