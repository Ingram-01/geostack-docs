Expressions
=====

.. _installation:

Basics
------------

Expressions are text/strings that you can use with Geostack for take control of a Property.

Every Expressions are located under any property that supported it.

.. figure:: images/expression_field.gif
  :width: 300
  :alt: Expression Field
  
  The black bars inside the red squares are all expression field.

.. figure:: videos/add_expression.gif
  :width: 400
  :alt: Add Expression

  To write an expression click with the mouse on the field and type what you need.

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']
