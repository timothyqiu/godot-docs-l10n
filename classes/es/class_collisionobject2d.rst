:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the CollisionObject2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_CollisionObject2D:

CollisionObject2D
=================

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`Area2D<class_Area2D>`, :ref:`PhysicsBody2D<class_PhysicsBody2D>`

Nodo base para objetos de colisión 2D.

Descripción
----------------------

CollisionObject2D es la clase base de los objetos de física 2D. Puede contener cualquier número de colisiones 2D :ref:`Shape2D<class_Shape2D>`. Cada forma debe ser asignada a un *propietario de la forma*. El CollisionObject2D puede tener cualquier número de propietarios de formas. Los propietarios de formas no son nodos y no aparecen en el editor, pero son accesibles a través del código usando los métodos ``shape_owner_*``.

Propiedades
----------------------

+-------------------------+--------------------------------------------------------------------------+----------+
| :ref:`int<class_int>`   | :ref:`collision_layer<class_CollisionObject2D_property_collision_layer>` | ``1``    |
+-------------------------+--------------------------------------------------------------------------+----------+
| :ref:`int<class_int>`   | :ref:`collision_mask<class_CollisionObject2D_property_collision_mask>`   | ``1``    |
+-------------------------+--------------------------------------------------------------------------+----------+
| :ref:`bool<class_bool>` | :ref:`input_pickable<class_CollisionObject2D_property_input_pickable>`   | ``true`` |
+-------------------------+--------------------------------------------------------------------------+----------+

Métodos
--------------

+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`_input_event<class_CollisionObject2D_method__input_event>` **(** :ref:`Object<class_Object>` viewport, :ref:`InputEvent<class_InputEvent>` event, :ref:`int<class_int>` shape_idx **)** |virtual| |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`create_shape_owner<class_CollisionObject2D_method_create_shape_owner>` **(** :ref:`Object<class_Object>` owner **)**                                                                              |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`get_collision_layer_bit<class_CollisionObject2D_method_get_collision_layer_bit>` **(** :ref:`int<class_int>` bit **)** |const|                                                                    |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`get_collision_mask_bit<class_CollisionObject2D_method_get_collision_mask_bit>` **(** :ref:`int<class_int>` bit **)** |const|                                                                      |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_RID>`                 | :ref:`get_rid<class_CollisionObject2D_method_get_rid>` **(** **)** |const|                                                                                                                              |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`             | :ref:`get_shape_owner_one_way_collision_margin<class_CollisionObject2D_method_get_shape_owner_one_way_collision_margin>` **(** :ref:`int<class_int>` owner_id **)** |const|                             |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`             | :ref:`get_shape_owners<class_CollisionObject2D_method_get_shape_owners>` **(** **)**                                                                                                                    |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`is_shape_owner_disabled<class_CollisionObject2D_method_is_shape_owner_disabled>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                               |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`               | :ref:`is_shape_owner_one_way_collision_enabled<class_CollisionObject2D_method_is_shape_owner_one_way_collision_enabled>` **(** :ref:`int<class_int>` owner_id **)** |const|                             |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`remove_shape_owner<class_CollisionObject2D_method_remove_shape_owner>` **(** :ref:`int<class_int>` owner_id **)**                                                                                 |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_collision_layer_bit<class_CollisionObject2D_method_set_collision_layer_bit>` **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**                                             |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`set_collision_mask_bit<class_CollisionObject2D_method_set_collision_mask_bit>` **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**                                               |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`shape_find_owner<class_CollisionObject2D_method_shape_find_owner>` **(** :ref:`int<class_int>` shape_index **)** |const|                                                                          |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_add_shape<class_CollisionObject2D_method_shape_owner_add_shape>` **(** :ref:`int<class_int>` owner_id, :ref:`Shape2D<class_Shape2D>` shape **)**                                      |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_clear_shapes<class_CollisionObject2D_method_shape_owner_clear_shapes>` **(** :ref:`int<class_int>` owner_id **)**                                                                     |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Object<class_Object>`           | :ref:`shape_owner_get_owner<class_CollisionObject2D_method_shape_owner_get_owner>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                                   |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Shape2D<class_Shape2D>`         | :ref:`shape_owner_get_shape<class_CollisionObject2D_method_shape_owner_get_shape>` **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|                                   |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`shape_owner_get_shape_count<class_CollisionObject2D_method_shape_owner_get_shape_count>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                       |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                 | :ref:`shape_owner_get_shape_index<class_CollisionObject2D_method_shape_owner_get_shape_index>` **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|                       |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Transform2D<class_Transform2D>` | :ref:`shape_owner_get_transform<class_CollisionObject2D_method_shape_owner_get_transform>` **(** :ref:`int<class_int>` owner_id **)** |const|                                                           |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_remove_shape<class_CollisionObject2D_method_shape_owner_remove_shape>` **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)**                                     |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_set_disabled<class_CollisionObject2D_method_shape_owner_set_disabled>` **(** :ref:`int<class_int>` owner_id, :ref:`bool<class_bool>` disabled **)**                                   |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_set_one_way_collision<class_CollisionObject2D_method_shape_owner_set_one_way_collision>` **(** :ref:`int<class_int>` owner_id, :ref:`bool<class_bool>` enable **)**                   |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_set_one_way_collision_margin<class_CollisionObject2D_method_shape_owner_set_one_way_collision_margin>` **(** :ref:`int<class_int>` owner_id, :ref:`float<class_float>` margin **)**   |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                  | :ref:`shape_owner_set_transform<class_CollisionObject2D_method_shape_owner_set_transform>` **(** :ref:`int<class_int>` owner_id, :ref:`Transform2D<class_Transform2D>` transform **)**                  |
+---------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Señales
--------------

.. _class_CollisionObject2D_signal_input_event:

- **input_event** **(** :ref:`Node<class_Node>` viewport, :ref:`InputEvent<class_InputEvent>` event, :ref:`int<class_int>` shape_idx **)**

Emitido cuando ocurre un evento de entrada. Requiere que :ref:`input_pickable<class_CollisionObject2D_property_input_pickable>` sea ``true`` y que se establezca al menos un bit ``collision_layer``. Ver :ref:`_input_event<class_CollisionObject2D_method__input_event>` para más detalles.

----

.. _class_CollisionObject2D_signal_mouse_entered:

- **mouse_entered** **(** **)**

Emitido cuando el puntero del ratón entra en cualquiera de las formas de este objeto. Requiere que :ref:`input_pickable<class_CollisionObject2D_property_input_pickable>` sea ``true`` y que al menos un bit ``collision_layer`` sea establecido.

----

.. _class_CollisionObject2D_signal_mouse_exited:

- **mouse_exited** **(** **)**

Emitido cuando el puntero del ratón sale de todas las formas de este objeto. Requiere que :ref:`input_pickable<class_CollisionObject2D_property_input_pickable>` sea ``true`` y que al menos un bit ``collision_layer`` esté activado.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_CollisionObject2D_property_collision_layer:

- :ref:`int<class_int>` **collision_layer**

+-----------+----------------------------+
| *Default* | ``1``                      |
+-----------+----------------------------+
| *Setter*  | set_collision_layer(value) |
+-----------+----------------------------+
| *Getter*  | get_collision_layer()      |
+-----------+----------------------------+

The physics layers this CollisionObject2D is in. Collision objects can exist in one or more of 32 different layers. See also :ref:`collision_mask<class_CollisionObject2D_property_collision_mask>`.

\ **Note:** A contact is detected if object A is in any of the layers that object B scans, or object B is in any layers that object A scans. See `Collision layers and masks <../tutorials/physics/physics_introduction.html#collision-layers-and-masks>`__ in the documentation for more information.

----

.. _class_CollisionObject2D_property_collision_mask:

- :ref:`int<class_int>` **collision_mask**

+-----------+---------------------------+
| *Default* | ``1``                     |
+-----------+---------------------------+
| *Setter*  | set_collision_mask(value) |
+-----------+---------------------------+
| *Getter*  | get_collision_mask()      |
+-----------+---------------------------+

The physics layers this CollisionObject2D scans. Collision objects can scan one or more of 32 different layers. See also :ref:`collision_layer<class_CollisionObject2D_property_collision_layer>`.

\ **Note:** A contact is detected if object A is in any of the layers that object B scans, or object B is in any layers that object A scans. See `Collision layers and masks <../tutorials/physics/physics_introduction.html#collision-layers-and-masks>`__ in the documentation for more information.

----

.. _class_CollisionObject2D_property_input_pickable:

- :ref:`bool<class_bool>` **input_pickable**

+-----------+---------------------+
| *Default* | ``true``            |
+-----------+---------------------+
| *Setter*  | set_pickable(value) |
+-----------+---------------------+
| *Getter*  | is_pickable()       |
+-----------+---------------------+

Si ``true``, este objeto es seleccionable. Un objeto seleccionable puede detectar el puntero del ratón entrando y saliendo, y si el ratón está dentro de él, informar de los eventos de entrada. Requiere al menos un bit ``collision_layer`` para ser establecido.

Descripciones de Métodos
------------------------------------------------

.. _class_CollisionObject2D_method__input_event:

- void **_input_event** **(** :ref:`Object<class_Object>` viewport, :ref:`InputEvent<class_InputEvent>` event, :ref:`int<class_int>` shape_idx **)** |virtual|

Acepta :ref:`InputEvent<class_InputEvent>`\ s no manipulados. Requiere que :ref:`input_pickable<class_CollisionObject2D_property_input_pickable>` sea ``true``. ``shape_idx`` es el índice hijo de la :ref:`Shape2D<class_Shape2D>` seleccionada. Conecta con la señal ``input_event`` para recoger fácilmente estos eventos.

----

.. _class_CollisionObject2D_method_create_shape_owner:

- :ref:`int<class_int>` **create_shape_owner** **(** :ref:`Object<class_Object>` owner **)**

Crea un nuevo dueño de la forma para el objeto dado. Devuelve ``owner_id`` del nuevo propietario para futuras referencias.

----

.. _class_CollisionObject2D_method_get_collision_layer_bit:

- :ref:`bool<class_bool>` **get_collision_layer_bit** **(** :ref:`int<class_int>` bit **)** |const|

Returns whether or not the specified ``bit`` of the :ref:`collision_layer<class_CollisionObject2D_property_collision_layer>` is set.

----

.. _class_CollisionObject2D_method_get_collision_mask_bit:

- :ref:`bool<class_bool>` **get_collision_mask_bit** **(** :ref:`int<class_int>` bit **)** |const|

Returns whether or not the specified ``bit`` of the :ref:`collision_mask<class_CollisionObject2D_property_collision_mask>` is set.

----

.. _class_CollisionObject2D_method_get_rid:

- :ref:`RID<class_RID>` **get_rid** **(** **)** |const|

Devuelve el :ref:`RID<class_RID>` del objeto.

----

.. _class_CollisionObject2D_method_get_shape_owner_one_way_collision_margin:

- :ref:`float<class_float>` **get_shape_owner_one_way_collision_margin** **(** :ref:`int<class_int>` owner_id **)** |const|

Devuelve el ``one_way_collision_margin`` del propietario de la forma identificado por el ``owner_id`` dado.

----

.. _class_CollisionObject2D_method_get_shape_owners:

- :ref:`Array<class_Array>` **get_shape_owners** **(** **)**

Devuelve un :ref:`Array<class_Array>` de identificadores ``owner_id``. Puedes usar estos identificadores en otros métodos que toman ``owner_id`` como argumento.

----

.. _class_CollisionObject2D_method_is_shape_owner_disabled:

- :ref:`bool<class_bool>` **is_shape_owner_disabled** **(** :ref:`int<class_int>` owner_id **)** |const|

Si ``true``, el propietario de la forma y sus formas se desactivan.

----

.. _class_CollisionObject2D_method_is_shape_owner_one_way_collision_enabled:

- :ref:`bool<class_bool>` **is_shape_owner_one_way_collision_enabled** **(** :ref:`int<class_int>` owner_id **)** |const|

Devuelve ``true`` si las colisiones para el propietario de la forma originadas por este ``CollisionObject2D`` no serán reportadas como colisionadas con los ``CollisionObject2D``\ s.

----

.. _class_CollisionObject2D_method_remove_shape_owner:

- void **remove_shape_owner** **(** :ref:`int<class_int>` owner_id **)**

Elimina al dueño de la forma dada.

----

.. _class_CollisionObject2D_method_set_collision_layer_bit:

- void **set_collision_layer_bit** **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**

If ``value`` is ``true``, sets the specified ``bit`` in the the :ref:`collision_layer<class_CollisionObject2D_property_collision_layer>`.

If ``value`` is ``false``, clears the specified ``bit`` in the the :ref:`collision_layer<class_CollisionObject2D_property_collision_layer>`.

----

.. _class_CollisionObject2D_method_set_collision_mask_bit:

- void **set_collision_mask_bit** **(** :ref:`int<class_int>` bit, :ref:`bool<class_bool>` value **)**

If ``value`` is ``true``, sets the specified ``bit`` in the the :ref:`collision_mask<class_CollisionObject2D_property_collision_mask>`.

If ``value`` is ``false``, clears the specified ``bit`` in the the :ref:`collision_mask<class_CollisionObject2D_property_collision_mask>`.

----

.. _class_CollisionObject2D_method_shape_find_owner:

- :ref:`int<class_int>` **shape_find_owner** **(** :ref:`int<class_int>` shape_index **)** |const|

Devuelve el ``owner_id`` de la forma dada.

----

.. _class_CollisionObject2D_method_shape_owner_add_shape:

- void **shape_owner_add_shape** **(** :ref:`int<class_int>` owner_id, :ref:`Shape2D<class_Shape2D>` shape **)**

Añade un :ref:`Shape2D<class_Shape2D>` al dueño de la forma.

----

.. _class_CollisionObject2D_method_shape_owner_clear_shapes:

- void **shape_owner_clear_shapes** **(** :ref:`int<class_int>` owner_id **)**

Elimina todas las formas del dueño de la forma.

----

.. _class_CollisionObject2D_method_shape_owner_get_owner:

- :ref:`Object<class_Object>` **shape_owner_get_owner** **(** :ref:`int<class_int>` owner_id **)** |const|

Devuelve el objeto padre del propietario de la forma dada.

----

.. _class_CollisionObject2D_method_shape_owner_get_shape:

- :ref:`Shape2D<class_Shape2D>` **shape_owner_get_shape** **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|

Devuelve el :ref:`Shape2D<class_Shape2D>` con la identificación dada por el dueño de la forma.

----

.. _class_CollisionObject2D_method_shape_owner_get_shape_count:

- :ref:`int<class_int>` **shape_owner_get_shape_count** **(** :ref:`int<class_int>` owner_id **)** |const|

Devuelve el número de formas que contiene el propietario de la forma dada.

----

.. _class_CollisionObject2D_method_shape_owner_get_shape_index:

- :ref:`int<class_int>` **shape_owner_get_shape_index** **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)** |const|

Devuelve el índice de hijos de la :ref:`Shape2D<class_Shape2D>` con el id dado del propietario de la forma.

----

.. _class_CollisionObject2D_method_shape_owner_get_transform:

- :ref:`Transform2D<class_Transform2D>` **shape_owner_get_transform** **(** :ref:`int<class_int>` owner_id **)** |const|

Devuelve la forma del dueño :ref:`Transform2D<class_Transform2D>`.

----

.. _class_CollisionObject2D_method_shape_owner_remove_shape:

- void **shape_owner_remove_shape** **(** :ref:`int<class_int>` owner_id, :ref:`int<class_int>` shape_id **)**

Quita una forma del dueño de la forma dada.

----

.. _class_CollisionObject2D_method_shape_owner_set_disabled:

- void **shape_owner_set_disabled** **(** :ref:`int<class_int>` owner_id, :ref:`bool<class_bool>` disabled **)**

Si ``true``, deshabilita al dueño de la forma dada.

----

.. _class_CollisionObject2D_method_shape_owner_set_one_way_collision:

- void **shape_owner_set_one_way_collision** **(** :ref:`int<class_int>` owner_id, :ref:`bool<class_bool>` enable **)**

Si ``enable`` es ``true``, las colisiones para el propietario de la forma originadas por este ``CollisionObject2D`` no se comunicarán como colisiones con las de ``CollisionObject2D``.

----

.. _class_CollisionObject2D_method_shape_owner_set_one_way_collision_margin:

- void **shape_owner_set_one_way_collision_margin** **(** :ref:`int<class_int>` owner_id, :ref:`float<class_float>` margin **)**

Establece el ``one_way_collision_margin`` del propietario de la forma identificado por el ``owner_id`` dado a los píxeles del ``margin``.

----

.. _class_CollisionObject2D_method_shape_owner_set_transform:

- void **shape_owner_set_transform** **(** :ref:`int<class_int>` owner_id, :ref:`Transform2D<class_Transform2D>` transform **)**

Establece la :ref:`Transform2D<class_Transform2D>` del propietario de la forma dada.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
