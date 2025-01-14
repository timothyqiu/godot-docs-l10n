:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the InstancePlaceholder.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_InstancePlaceholder:

InstancePlaceholder
===================

**Inherits:** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

:ref:`PackedScene<class_PackedScene>` 根 :ref:`Node<class_Node>` 的占位。

描述
----

在编辑器中为实例化场景打开选项 **加载为占位符** 会导致在运行游戏时将其替换为实例占位符\ ``InstancePlaceholder``\ 。这使得实际加载场景的时间可以推迟到调用\ :ref:`replace_by_instance<class_InstancePlaceholder_method_replace_by_instance>`\ 。这对于通过选择性加载部分场景来避免一次性加载大场景很有用。

实例占位符没有变换(transform)属性。这导致任何子节点从点（0,0）开始相对于视窗进行定位，而不是在编辑器中显示的父节点。用一个具有变换属性的场景来替换占位符，将使子节点再次相对于它们的父节点进行变换。

方法
----

+-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Node<class_Node>`             | :ref:`create_instance<class_InstancePlaceholder_method_create_instance>` **(** :ref:`bool<class_bool>` replace=false, :ref:`PackedScene<class_PackedScene>` custom_scene=null **)** |
+-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`         | :ref:`get_instance_path<class_InstancePlaceholder_method_get_instance_path>` **(** **)** |const|                                                                                    |
+-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Dictionary<class_Dictionary>` | :ref:`get_stored_values<class_InstancePlaceholder_method_get_stored_values>` **(** :ref:`bool<class_bool>` with_order=false **)**                                                   |
+-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                | :ref:`replace_by_instance<class_InstancePlaceholder_method_replace_by_instance>` **(** :ref:`PackedScene<class_PackedScene>` custom_scene=null **)**                                |
+-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

方法说明
--------

.. _class_InstancePlaceholder_method_create_instance:

- :ref:`Node<class_Node>` **create_instance** **(** :ref:`bool<class_bool>` replace=false, :ref:`PackedScene<class_PackedScene>` custom_scene=null **)**

不是线程安全的。如果从线程调用，请使用\ :ref:`Object.call_deferred<class_Object_method_call_deferred>`\ 。

----

.. _class_InstancePlaceholder_method_get_instance_path:

- :ref:`String<class_String>` **get_instance_path** **(** **)** |const|

获取调用 :ref:`replace_by_instance<class_InstancePlaceholder_method_replace_by_instance>` 时默认加载的 :ref:`PackedScene<class_PackedScene>` 资源文件的路径。不是线程安全的。如果从线程调用，请使用\ :ref:`Object.call_deferred<class_Object_method_call_deferred>`\ 。

----

.. _class_InstancePlaceholder_method_get_stored_values:

- :ref:`Dictionary<class_Dictionary>` **get_stored_values** **(** :ref:`bool<class_bool>` with_order=false **)**

----

.. _class_InstancePlaceholder_method_replace_by_instance:

- void **replace_by_instance** **(** :ref:`PackedScene<class_PackedScene>` custom_scene=null **)**

用作为参数的场景替换这个占位符，如果没有给出参数，则替换原始场景。对于所有的资源来说，只有当场景还没有被加载时才会被加载。通过事先手动加载场景，可以避免由这个函数引起的延迟。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
