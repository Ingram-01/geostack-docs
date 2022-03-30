Expressions
=====

Basics
------------

| Expressions are text/strings that you can use with Geostack for take control of a property.  
| They are located under any property that supported it.

.. figure:: images/expression_field_2.jpg
  :width: 400
  :alt: Expression Field
  
  A property and an expression field.

To write an expression click with the mouse on the field and type what you need.

.. figure:: videos/add_expression.gif
  :width: 400
  :alt: Add Expression

  In this example we simply write a single value to the expression field

| Expressions support: :ref:`values`, :ref:`operators`, :ref:`maths`, :ref:`links`, :ref:`arrays`, :ref:`builtin` and :ref:`constants`.
| You can concatenates all of this until you get the desired result.
| It's similar when you use a Nodes Editor and you link outputs and inputs but, instead to use nodes, you use text.
.. Expressions are basicaly the text way to do spaghetti nodes.
|
| Let's make an example:

.. figure:: videos/sine_movement.gif
  :width: 200
  :alt: Sine Movement
  :align: center

  A cube that move up and down.

.. figure:: images/sine_movement_gn_gs.jpg
  :width: 700
  :alt: Sine Movement Geometry Nodes
  :align: center

  On the left is how you make the movement in Geometry Nodes on the right in Geostack.

.. _values:

Values
------------

.. _float:

------------
Float
------------

Floating point real values: 0.5, 1.0, 2.1 ecc...

------------
Int
------------

Signed Integer: 1, 2, 3, 4 ecc..

------------
Bool
------------

| Booleans represent one of two values: True or False.
| Usefull in :ref:`ternary`.

------------
Vector
------------

| Representation of 3D vectors.
| You can use them in expressions as v( x, y, z ).

.. figure:: videos/vector.gif
  :width: 400
  :alt: Add Expression
  
  Example of a new vector.

------------
Euler
------------

Representation of 3D vectors and points as x,y,z

.. _builtin:

Built-In Functions
------------

| Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow
| Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow
| Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _constants:

------------
Constants
------------

Constants are Built-In fixed variables that you can use whatever you want.

.. figure:: videos/constants_1.gif
  :width: 400
  :alt: Constants

  An example of constants

------------
Slot Reference
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _maths:

------------
Maths
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _operators:

------------
Operators
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _ternary:

------------
Ternary
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _links:

Links
------------

.. _links_basics:

------------
Basics
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _arrays:

------------
Arrays
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _links_expressions:

------------
Expression
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _object:

------------
Object
----------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. 
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
    .. py:data:: Int
