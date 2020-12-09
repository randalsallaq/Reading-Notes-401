# Dunder (Magic, Special) Methods
#### Dunder or magic methods in Python are the methods having two prefix and suffix underscores in the method name. Dunder here means “Double Under (Underscores)”. These are commonly used for operator overloading

![d](https://www.python-course.eu/images/marvin_the_magician.png)


- ***Object Initialization:
 __init__***:
 
 
 ```def __init__(self, owner, amount=0):
        """
        This is the constructor that lets us create
        objects from this class
        """
        self.owner = owner
        self.amount = amount
        self._transactions =[]```
        
        
        
         
 - ***Object Representation:
 __str__, __repr__***:
 
 
 ```def __repr__(self):
        return 'Account({!r}, {!r})'.format(self.owner, self.amount)

    def __str__(self):
        return 'Account of {} with starting amount: {}'.format(
            self.owner, self.amount)```
 
 
 - ***Iteration:
 __len__, __getitem__, __reversed__***:
 
 ```ef __reversed__(self):
    return self[::-1]

>>> list(reversed(acc))
[30, -20, 50, -10, 20]```
 
 
 
- ***Operator Overloading for Comparing Accounts:
__eq__, __lt__***:

 ```from functools import total_ordering
@total_ordering
class Account:
    def __eq__(self, other):
        return self.balance == other.balance

    def __lt__(self, other):
        return self.balance < other.balance```
 
 
 - ***Operator Overloading for Merging Accounts:
 __add__***:
 
  ```def __add__(self, other):
    owner = self.owner + other.owner
    start_amount = self.balance + other.balance
    return Account(owner, start_amount)```
 
 
 
 - ***Callable Python Objects:
 __call__***:
 
 ```class Account:
    # ... (see above)

    def __call__(self):
        print('Start amount: {}'.format(self.amount))
        print('Transactions: ')
        for transaction in self:
            print(transaction)
        print('\nBalance: {}'.format(self.balance))```
 
 
