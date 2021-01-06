The default User model in Django uses a username to uniquely identify a user during authentication. If you'd rather use an email address, you'll need to create a custom User model by either subclassing AbstractUser or AbstractBaseUser.

Options:

AbstractUser: Use this option if you are happy with the existing fields on the User model and just want to remove the username field.
AbstractBaseUser: Use this option if you want to start from scratch by creating your own, completely new User model.
We'll look at both options, AbstractUser and AbstractBaseUser, in this post.

The steps are the same for each:

Create a custom User model and Manager
Update settings.py
Customize the UserCreationForm and UserChangeForm forms
Update the admin

![u](https://miro.medium.com/max/491/1*I41KMqFd4Lz9Nom_ga7nkg.png)
