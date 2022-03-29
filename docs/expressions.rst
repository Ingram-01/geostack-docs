Expressions
=====

.. _installation:

How To
------------

Expressions are text/strings that you can use with Geostack for set a Property.

Every expressions field are located under any Property that supoorted it.

.. image:: images/expression_field.jpg
  :width: 400
  :alt: Expression Field

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
