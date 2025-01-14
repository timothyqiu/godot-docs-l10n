:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the BitMap.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_BitMap:

BitMap
======

**Inherits:** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Matriz booleana.

Descripción
----------------------

Una matriz bidimensional de valores booleanos, puede ser usada para almacenar eficientemente una matriz binaria (cada elemento de la matriz toma sólo un bit) y consultar los valores usando coordenadas cartesianas naturales.

Métodos
--------------

+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`create<class_BitMap_method_create>` **(** :ref:`Vector2<class_Vector2>` size **)**                                                                         |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`create_from_image_alpha<class_BitMap_method_create_from_image_alpha>` **(** :ref:`Image<class_Image>` image, :ref:`float<class_float>` threshold=0.1 **)** |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`get_bit<class_BitMap_method_get_bit>` **(** :ref:`Vector2<class_Vector2>` position **)** |const|                                                           |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_size<class_BitMap_method_get_size>` **(** **)** |const|                                                                                                |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_true_bit_count<class_BitMap_method_get_true_bit_count>` **(** **)** |const|                                                                            |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`grow_mask<class_BitMap_method_grow_mask>` **(** :ref:`int<class_int>` pixels, :ref:`Rect2<class_Rect2>` rect **)**                                         |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`     | :ref:`opaque_to_polygons<class_BitMap_method_opaque_to_polygons>` **(** :ref:`Rect2<class_Rect2>` rect, :ref:`float<class_float>` epsilon=2.0 **)** |const|      |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_bit<class_BitMap_method_set_bit>` **(** :ref:`Vector2<class_Vector2>` position, :ref:`bool<class_bool>` bit **)**                                      |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_bit_rect<class_BitMap_method_set_bit_rect>` **(** :ref:`Rect2<class_Rect2>` rect, :ref:`bool<class_bool>` bit **)**                                    |
+-------------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Descripciones de Métodos
------------------------------------------------

.. _class_BitMap_method_create:

- void **create** **(** :ref:`Vector2<class_Vector2>` size **)**

Crea un mapa de bits con el tamaño especificado, lleno de ``false``.

----

.. _class_BitMap_method_create_from_image_alpha:

- void **create_from_image_alpha** **(** :ref:`Image<class_Image>` image, :ref:`float<class_float>` threshold=0.1 **)**

Crea un mapa de bits que coincide con las dimensiones de la imagen dada, cada elemento del mapa de bits se establece en ``false`` si el valor alfa de la imagen en esa posición es igual al umbral ``threshold`` o menor, y ``true`` en otro caso.

----

.. _class_BitMap_method_get_bit:

- :ref:`bool<class_bool>` **get_bit** **(** :ref:`Vector2<class_Vector2>` position **)** |const|

Devuelve el valor del mapa de bits en la posición especificada.

----

.. _class_BitMap_method_get_size:

- :ref:`Vector2<class_Vector2>` **get_size** **(** **)** |const|

Devuelve las dimensiones del mapa de bits.

----

.. _class_BitMap_method_get_true_bit_count:

- :ref:`int<class_int>` **get_true_bit_count** **(** **)** |const|

Devuelve la cantidad de elementos de mapa de bits que están configurados a ``true``.

----

.. _class_BitMap_method_grow_mask:

- void **grow_mask** **(** :ref:`int<class_int>` pixels, :ref:`Rect2<class_Rect2>` rect **)**

Applies morphological dilation or erosion to the bitmap. If ``pixels`` is positive, dilation is applied to the bitmap. If ``pixels`` is negative, erosion is applied to the bitmap. ``rect`` defines the area where the morphological operation is applied. Pixels located outside the ``rect`` are unaffected by :ref:`grow_mask<class_BitMap_method_grow_mask>`.

----

.. _class_BitMap_method_opaque_to_polygons:

- :ref:`Array<class_Array>` **opaque_to_polygons** **(** :ref:`Rect2<class_Rect2>` rect, :ref:`float<class_float>` epsilon=2.0 **)** |const|

----

.. _class_BitMap_method_set_bit:

- void **set_bit** **(** :ref:`Vector2<class_Vector2>` position, :ref:`bool<class_bool>` bit **)**

Establece el elemento del mapa de bits en la posición especificada, al valor especificado.

----

.. _class_BitMap_method_set_bit_rect:

- void **set_bit_rect** **(** :ref:`Rect2<class_Rect2>` rect, :ref:`bool<class_bool>` bit **)**

Establece una porción rectangular del mapa de bits al valor especificado.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
