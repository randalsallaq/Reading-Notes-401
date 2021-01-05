# Django Form

### A ModelForm maps a model class's fields to HTML form <input> elements via a Form ; this is what the Django admin is based upon. A form's fields are themselves classes; they manage form data and perform validation when a form is submitted.

![r](https://cdn.swapps.com/uploads/2018/09/how-to-do-a-wizard-form-with-django.jpg)


## Django form structure and workflow:

![f](https://www.webforefront.com/static/images/beginningdjango/Figure_6-1.png)


## Django’s role in forms:

Django handles three distinct parts of the work involved in forms:

- preparing and restructuring data to make it ready for rendering
- creating HTML forms for the data
- receiving and processing submitted forms and data from the client


## Instantiating, processing, and rendering forms

- get hold of it in the view
- pass it to the template context
- expand it to HTML markup using template variables

![d](https://mdn.mozillademos.org/files/14205/Form%20Handling%20-%20Standard.png)
