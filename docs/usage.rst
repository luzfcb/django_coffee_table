========
Usage
========

To use coffee_table in your project:

1. Set up dependencies according to their respective documentation:

* `linaro-django-pagination <https://pypi.python.org/pypi/linaro-django-pagination/>`_
* `django-resort <https://pypi.python.org/pypi/django_resort/0.1.0>`_
* `django-tag-parser <https://pypi.python.org/pypi/django-tag-parser>`_

2. Include `django_coffee_table` in your `INSTALLED_APPS`.

3. Open your template and load up the coffee_table tags library::

		{% load coffee_table %}

4. Basic usage::

		{% coffee_table object_list %}

5. Advanced usage::

		{% coffee_table object_list field_accessors='name, content_type__app_label'
																paginate_by='10'
																table_class='table table-condensed'
																checkbox_column=True
																primary_key_column=True
																help_text=True %}

Please see the included test project for more help.
