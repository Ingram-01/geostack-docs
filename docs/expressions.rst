Expressions
=====

Basics
------------

| Expressions are text/strings that you can use with Geostack to take control of a property.
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
| You can concatenate all of this until you get the desired result.
| It is similar when you use a node editor and link outputs and inputs but, instead of using nodes, you use text.
| Let's make an example:

.. figure:: videos/sine_movement.gif
  :width: 200
  :alt: Sine Movement
  :align: center

  A cube that float up and down.

.. figure:: images/sine_movement_gn_gs.jpg
  :width: 700
  :alt: Sine Movement Geometry Nodes
  :align: center

  On the left the Geometry Nodes version of the movement on the right the Geostack one.

.. _values:

Values
------------

.. _float:

------------
Float
------------

Floating point real values: 0.5, 1.0, 2.1 etc...

.. _int:

------------
Int
------------

Signed Integer: 1, 2, 3, 4 etc..

.. _bool:

------------
Bool
------------

| Booleans represent one of two values: True or False.
| Usefull in :ref:`ternary`.

.. _vector:

------------
Vector
------------

| 3D vector with floating-point values.
| You can use them in expressions as v(x,y,z) or x,y,z if you only need one single value.

.. figure:: videos/vector.gif
  :width: 300
  :alt: Add Expression
  
  Example of a new vector.
  
| Vectors support almost all operations and also support all functions of the `Python Blender Api`_
| If you want to learn, more `here`_.

.. _here: https://docs.blender.org/api/current/mathutils.html#mathutils.Vector

.. _Python Blender Api: https://docs.blender.org/api/current/index.html

.. _euler:

------------
Euler
------------

Representation of 3D vectors and points as x,y,z

.. _builtin:

Built-In Functions and Constants
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
  :align: center

  An example of constants.

This is the list of all constants (more elements in the next updates)

.. py:data:: v_zero 

    A Zero :ref:`vector` = v(0,0,0)

.. py:data:: v_one 

    A One :ref:`vector` = v(1,1,1)

.. py:data:: v_half 

    An half :ref:`vector` = v(0.5,0.5,0.5)

.. py:data:: v_up 

    Directional up :ref:`vector` = v(0,0,1)

.. py:data:: v_down 

    Directional down :ref:`vector` = v(0,0,-1)

.. py:data:: v_right 

    Directional right :ref:`vector` = v(1,0,0)

.. py:data:: v_left 

    Directional left :ref:`vector` = v(-1,0,0)

.. py:data:: v_for 

    Directional forward :ref:`vector` = v(0,1,0)

.. py:data:: v_back 

    Directional backward :ref:`vector` = v(0,-1,0)

.. py:data:: v_yz 

    0XY :ref:`vector` = v(0,1,1)

.. py:data:: v_xz 

    X0Z :ref:`vector` = v(1,0,1)

.. py:data:: v_xy 

    XY0 :ref:`vector` = v(1,1,0)

.. py:data:: e_zero 

    A Zero :ref:`euler` = e(0,0,0)

.. py:data:: e_x45

    A X 45° :ref:`euler` = e(45,0,0)

.. py:data:: e_x90

    A X 90° :ref:`euler` = e(90,0,0)

.. py:data:: e_x180

    A X 180° :ref:`euler` = e(180,0,0)

.. py:data:: e_y45

    A Y 45° :ref:`euler` = e(0,45,0)

.. py:data:: e_y90

    A Y 90° :ref:`euler` = e(0,90,0)

.. py:data:: e_y180

    A Y 180° :ref:`euler` = e(0,180,0)

.. py:data:: e_z45

    A Z 45° :ref:`euler` = e(0,0,45)

.. py:data:: e_z90

    A Z 90° :ref:`euler` = e(0,0,90)

.. py:data:: e_z180

    A Z 180° :ref:`euler` = e(0,0,180)

.. py:data:: epsilon

    Epsilon number :ref:`float` = 0.00001


------------
Slot Get
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

| Links are custom global properties that you can use whatever you want in expressions.
| They can be managed easily in the links panel.

.. figure:: images/links.jpg
  :width: 300
  :alt: Link Panel

| Links have a naming convention and have two rules:
| 1 - Every links name must be a Title Case (so no lower case for the first character). 
| 2 - The only special character allowed is the Underscore, so no points, signs, or parenthesis.

* Links types are:
  
  * :ref:`float`
  * :ref:`int`
  * :ref:`bool`
  * :ref:`vector`
  * :ref:`euler`
  * :ref:`transform`
  * :ref:`links_expressions`
  * :ref:`object`
  * :ref:`link_lists`

.. _link_lists:

------------
Lists
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
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _transform:

------------
Transform
------------

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
    .. Expressions are basicaly the text way to do spaghetti nodes.

    "v_zero = x:0 y:0 z:0
    "v_one = x:1 y:1 z:1
    "v_half = x:0.5 y:0.5 z:0.5
    "v_half_up = x:0.5 y:0.5 z:1
    "v_xy = x:1 y:1 z:0
    "v_yz = x:0 y:1 z:1
    "v_xz = x:1 y:0 z:1 \n",
    "v_up = x:0 y:0 z:1 \n",
    "v_down = x:0 y:0 z:-1 \n",
    "v_right = x:1 y:0 z:0 \n",
    "v_left = x:-1 y:0 z:0 \n",
    "v_for = x:0 y:1 z:0 \n",
    "v_back = x:0 y:-1 z:0 \n",
    "e_zero = x:0 y:0 z:0 \n",
    "epsilon = 0.00001 \n",
