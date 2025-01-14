:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the AABB.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_AABB:

AABB
====

轴对齐包围盒。

描述
----

``AABB`` consists of a position, a size, and several utility functions. It is typically used for fast overlap tests.

It uses floating-point coordinates. The 2D counterpart to ``AABB`` is :ref:`Rect2<class_Rect2>`.

Negative values for :ref:`size<class_AABB_property_size>` are not supported and will not work for most methods. Use :ref:`abs<class_AABB_method_abs>` to get an AABB with a positive size.

\ **Note:** Unlike :ref:`Rect2<class_Rect2>`, ``AABB`` does not have a variant that uses integer coordinates.

教程
----

- :doc:`Math tutorial index <../tutorials/math/index>`

- :doc:`Vector math <../tutorials/math/vector_math>`

- :doc:`Advanced vector math <../tutorials/math/vectors_advanced>`

属性
----

+-------------------------------+-----------------------------------------------+------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`end<class_AABB_property_end>`           | ``Vector3( 0, 0, 0 )`` |
+-------------------------------+-----------------------------------------------+------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`position<class_AABB_property_position>` | ``Vector3( 0, 0, 0 )`` |
+-------------------------------+-----------------------------------------------+------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`size<class_AABB_property_size>`         | ``Vector3( 0, 0, 0 )`` |
+-------------------------------+-----------------------------------------------+------------------------+

方法
----

+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`       | :ref:`AABB<class_AABB_method_AABB>` **(** :ref:`Vector3<class_Vector3>` position, :ref:`Vector3<class_Vector3>` size **)**                       |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`       | :ref:`abs<class_AABB_method_abs>` **(** **)**                                                                                                    |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`encloses<class_AABB_method_encloses>` **(** :ref:`AABB<class_AABB>` with **)**                                                             |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`       | :ref:`expand<class_AABB_method_expand>` **(** :ref:`Vector3<class_Vector3>` to_point **)**                                                       |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`get_area<class_AABB_method_get_area>` **(** **)**                                                                                          |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`get_center<class_AABB_method_get_center>` **(** **)**                                                                                      |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`get_endpoint<class_AABB_method_get_endpoint>` **(** :ref:`int<class_int>` idx **)**                                                        |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`get_longest_axis<class_AABB_method_get_longest_axis>` **(** **)**                                                                          |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_longest_axis_index<class_AABB_method_get_longest_axis_index>` **(** **)**                                                              |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`get_longest_axis_size<class_AABB_method_get_longest_axis_size>` **(** **)**                                                                |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`get_shortest_axis<class_AABB_method_get_shortest_axis>` **(** **)**                                                                        |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_shortest_axis_index<class_AABB_method_get_shortest_axis_index>` **(** **)**                                                            |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`     | :ref:`get_shortest_axis_size<class_AABB_method_get_shortest_axis_size>` **(** **)**                                                              |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector3<class_Vector3>` | :ref:`get_support<class_AABB_method_get_support>` **(** :ref:`Vector3<class_Vector3>` dir **)**                                                  |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`       | :ref:`grow<class_AABB_method_grow>` **(** :ref:`float<class_float>` by **)**                                                                     |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`has_no_area<class_AABB_method_has_no_area>` **(** **)**                                                                                    |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`has_no_surface<class_AABB_method_has_no_surface>` **(** **)**                                                                              |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`has_point<class_AABB_method_has_point>` **(** :ref:`Vector3<class_Vector3>` point **)**                                                    |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`       | :ref:`intersection<class_AABB_method_intersection>` **(** :ref:`AABB<class_AABB>` with **)**                                                     |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`intersects<class_AABB_method_intersects>` **(** :ref:`AABB<class_AABB>` with **)**                                                         |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`intersects_plane<class_AABB_method_intersects_plane>` **(** :ref:`Plane<class_Plane>` plane **)**                                          |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`intersects_segment<class_AABB_method_intersects_segment>` **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to **)** |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`       | :ref:`is_equal_approx<class_AABB_method_is_equal_approx>` **(** :ref:`AABB<class_AABB>` aabb **)**                                               |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`       | :ref:`merge<class_AABB_method_merge>` **(** :ref:`AABB<class_AABB>` with **)**                                                                   |
+-------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------+

属性说明
--------

.. _class_AABB_property_end:

- :ref:`Vector3<class_Vector3>` **end**

+-----------+------------------------+
| *Default* | ``Vector3( 0, 0, 0 )`` |
+-----------+------------------------+

终点角。通过 ``position + size`` 计算而来。设置该值会修改大小。

----

.. _class_AABB_property_position:

- :ref:`Vector3<class_Vector3>` **position**

+-----------+------------------------+
| *Default* | ``Vector3( 0, 0, 0 )`` |
+-----------+------------------------+

起点角。通常比 :ref:`end<class_AABB_property_end>` 小。

----

.. _class_AABB_property_size:

- :ref:`Vector3<class_Vector3>` **size**

+-----------+------------------------+
| *Default* | ``Vector3( 0, 0, 0 )`` |
+-----------+------------------------+

从\ :ref:`position<class_AABB_property_position>` 到 :ref:`end<class_AABB_property_end>` 的大小。通常所有分量都是正数。

如果大小为负，可以用 :ref:`abs<class_AABB_method_abs>` 修正。

方法说明
--------

.. _class_AABB_method_AABB:

- :ref:`AABB<class_AABB>` **AABB** **(** :ref:`Vector3<class_Vector3>` position, :ref:`Vector3<class_Vector3>` size **)**

从一个位置和大小构造 ``AABB`` 。

----

.. _class_AABB_method_abs:

- :ref:`AABB<class_AABB>` **abs** **(** **)**

返回等价的 AABB，其原点被修正至最负数的角落，大小被修正为正数。

----

.. _class_AABB_method_encloses:

- :ref:`bool<class_bool>` **encloses** **(** :ref:`AABB<class_AABB>` with **)**

该 ``AABB`` 完全包含另一个时，返回 ``true``\ 。

----

.. _class_AABB_method_expand:

- :ref:`AABB<class_AABB>` **expand** **(** :ref:`Vector3<class_Vector3>` to_point **)**

返回该 ``AABB`` 的副本，该副本扩展至包含给出的点。

\ **例子：**\ 

::

    # position (-3, 2, 0), size (1, 1, 1)
    var box = AABB(Vector3(-3, 2, 0), Vector3(1, 1, 1))
    # position (-3, -1, 0), size (3, 4, 2), 包含原来的 AABB 和 Vector3(0, -1, 2)
    var box2 = box.expand(Vector3(0, -1, 2))

----

.. _class_AABB_method_get_area:

- :ref:`float<class_float>` **get_area** **(** **)**

返回该 ``AABB`` 的体积。

----

.. _class_AABB_method_get_center:

- :ref:`Vector3<class_Vector3>` **get_center** **(** **)**

Returns the center of the ``AABB``, which is equal to :ref:`position<class_AABB_property_position>` + (:ref:`size<class_AABB_property_size>` / 2).

----

.. _class_AABB_method_get_endpoint:

- :ref:`Vector3<class_Vector3>` **get_endpoint** **(** :ref:`int<class_int>` idx **)**

获取该 ``AABB`` 的 8 个端点的位置。

----

.. _class_AABB_method_get_longest_axis:

- :ref:`Vector3<class_Vector3>` **get_longest_axis** **(** **)**

返回该 ``AABB`` 归一化后的最长轴。

----

.. _class_AABB_method_get_longest_axis_index:

- :ref:`int<class_int>` **get_longest_axis_index** **(** **)**

返回该 ``AABB`` 最长轴的索引（根据 :ref:`Vector3<class_Vector3>` 的 ``AXIS_*`` 常量）。

----

.. _class_AABB_method_get_longest_axis_size:

- :ref:`float<class_float>` **get_longest_axis_size** **(** **)**

返回该 ``AABB`` 最长轴的标量长度。

----

.. _class_AABB_method_get_shortest_axis:

- :ref:`Vector3<class_Vector3>` **get_shortest_axis** **(** **)**

返回该 ``AABB`` 归一化后的最短轴。

----

.. _class_AABB_method_get_shortest_axis_index:

- :ref:`int<class_int>` **get_shortest_axis_index** **(** **)**

返回该 ``AABB`` 最短轴的索引（根据 :ref:`Vector3<class_Vector3>` 的 ``AXIS_*`` 常量）。

----

.. _class_AABB_method_get_shortest_axis_size:

- :ref:`float<class_float>` **get_shortest_axis_size** **(** **)**

返回该 ``AABB`` 最短轴的标量长度。

----

.. _class_AABB_method_get_support:

- :ref:`Vector3<class_Vector3>` **get_support** **(** :ref:`Vector3<class_Vector3>` dir **)**

返回指定方向上的支持点。常用于碰撞检测算法。

----

.. _class_AABB_method_grow:

- :ref:`AABB<class_AABB>` **grow** **(** :ref:`float<class_float>` by **)**

返回该 ``AABB`` 的副本，沿着所有面的方向都增加了指定的大小。

----

.. _class_AABB_method_has_no_area:

- :ref:`bool<class_bool>` **has_no_area** **(** **)**

该 ``AABB`` 为平面或者为空时，返回 ``true``\ 。

----

.. _class_AABB_method_has_no_surface:

- :ref:`bool<class_bool>` **has_no_surface** **(** **)**

该 ``AABB`` 为空时，返回 ``true``\ 。

----

.. _class_AABB_method_has_point:

- :ref:`bool<class_bool>` **has_point** **(** :ref:`Vector3<class_Vector3>` point **)**

该 ``AABB`` 包含指定点时，返回 ``true``\ 。

----

.. _class_AABB_method_intersection:

- :ref:`AABB<class_AABB>` **intersection** **(** :ref:`AABB<class_AABB>` with **)**

返回两个 ``AABB`` 的交叠区域。失败时返回空的 AABB（大小为 0,0,0）。

----

.. _class_AABB_method_intersects:

- :ref:`bool<class_bool>` **intersects** **(** :ref:`AABB<class_AABB>` with **)**

该 ``AABB`` 与另一个交叠时，返回 ``true``\ 。

----

.. _class_AABB_method_intersects_plane:

- :ref:`bool<class_bool>` **intersects_plane** **(** :ref:`Plane<class_Plane>` plane **)**

该 ``AABB`` 同时位于指定平面的两边时，返回 ``true``\ 。

----

.. _class_AABB_method_intersects_segment:

- :ref:`bool<class_bool>` **intersects_segment** **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to **)**

该 ``AABB`` 与 ``from`` 和 ``to`` 所构成的线段有交叠时，返回 ``true``\ 。

----

.. _class_AABB_method_is_equal_approx:

- :ref:`bool<class_bool>` **is_equal_approx** **(** :ref:`AABB<class_AABB>` aabb **)**

该 ``AABB`` 与 ``aabb`` 近似相等时，返回 ``true``\ 。通过将各个分量调用 :ref:`@GDScript.is_equal_approx<class_@GDScript_method_is_equal_approx>` 确定。

----

.. _class_AABB_method_merge:

- :ref:`AABB<class_AABB>` **merge** **(** :ref:`AABB<class_AABB>` with **)**

返回同时包含该 ``AABB`` 和 ``with`` 的更大的 ``AABB``\ 。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
