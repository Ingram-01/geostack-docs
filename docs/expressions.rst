Expressions
=====

Basics
------------

.. _Geostack: https://geostack-docs.readthedocs.io/en/latest/index.html

| Expressions are text/strings that you can use with `Geostack`_ to take control of a property.
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
| It is similar when you link inputs and outputs in a node editor but, instead of using nodes, you use text.
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
  
| Vectors support almost all operations and also support all functions of the `Python Blender API`_
| If you want to learn, more `here <https://docs.blender.org/api/current/mathutils.html#mathutils.Vector>`_.

.. _Python Blender API: https://docs.blender.org/api/current/index.html

.. _euler:

------------
Euler
------------

Representation of 3D vectors and points as x,y,z.

.. _object:

------------
Object
------------

| A Blender Object reference. Supports almost all blender properties.
| You can use it with links like this:
| *image here*
| More `here <https://docs.blender.org/api/current/bpy.types.Object.html#bpy.types.Object>`_.

.. _transform:

------------
Transform
------------

| Transform is a property that contain:
|   Location :ref:`vector`
|   Rotation :ref:`euler`
|   Size :ref:`vector`

| You can use it with links like this:
| *image here*

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

| Constants are read-only Built-In variables that you can use whatever you want.

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

| This is are a compact version functions of `python maths module <https://docs.python.org/3/library/math.html>`_.
| If you need a function that is not present in this list you can try with write *math.* before the function, but be aware that can give you an error.

.. py:function:: sin(x)

.. py:function:: cos(x)

.. py:function:: sqrt(x)

.. py:function:: floor(x)

.. py:function:: fmod(x)

.. py:function:: acos(x)

.. py:function:: ceil(x)

.. py:function:: pow(x)

.. py:function:: sqrt(x)

.. py:function:: atan(x)

.. py:function:: radians(x)

.. py:function:: tan(x)

.. py:function:: degrees(x)

.. py:function:: atan2(y, x)

.. py:function:: factorial(x)

.. py:function:: fmod(x)

.. py:function:: frexp(x)

.. py:function:: log10(x)

.. py:function:: log(x)

.. py:function:: log2(x)

.. py:function:: log1p(x)

.. py:function:: exp(x)

.. py:function:: expm1(x)

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
Link Lists
------------

Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow Meow

.. _links_expressions:

------------
Link Expression
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

    This is for the basics math
    | One of the pillars of `Geostack`_ expressions are the compactness. You can only write you
