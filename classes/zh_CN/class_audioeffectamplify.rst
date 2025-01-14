:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the AudioEffectAmplify.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_AudioEffectAmplify:

AudioEffectAmplify
==================

**Inherits:** :ref:`AudioEffect<class_AudioEffect>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

给音频总线添加放大音频效果。

增加或减少所选音频总线的音量。

描述
----

增加或减少通过音频总线传送的音量。

属性
----

+---------------------------+---------------------------------------------------------------+---------+
| :ref:`float<class_float>` | :ref:`volume_db<class_AudioEffectAmplify_property_volume_db>` | ``0.0`` |
+---------------------------+---------------------------------------------------------------+---------+

属性说明
--------

.. _class_AudioEffectAmplify_property_volume_db:

- :ref:`float<class_float>` **volume_db**

+-----------+----------------------+
| *Default* | ``0.0``              |
+-----------+----------------------+
| *Setter*  | set_volume_db(value) |
+-----------+----------------------+
| *Getter*  | get_volume_db()      |
+-----------+----------------------+

以分贝为单位的放大量。正值使声音更响亮，负值使声音更安静。数值范围从-80到24。

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
