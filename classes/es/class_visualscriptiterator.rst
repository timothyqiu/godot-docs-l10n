:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualScriptIterator.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualScriptIterator:

VisualScriptIterator
====================

**Inherits:** :ref:`VisualScriptNode<class_VisualScriptNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Pasos a través de los elementos de una entrada dada.

Descripción
----------------------

Este nodo pasa por cada elemento de una entrada determinada. La entrada puede ser de cualquier tipo de datos de secuencia, como un :ref:`Array<class_Array>` o una :ref:`String<class_String>`. Cuando cada elemento ha sido procesado, la ejecución pasa por el puerto de secuencia ``exit``.

\ **Puertos de entrada:**\ 

- Secuencia: ``for (elem) in (input)``\ 

- Datos (variante): ``input``\ 

\ **Puertos de salida:**\ 

- Secuencia: ``each``\ 

- Secuencia: ``exit``\ 

- Datos (variante): ``elem``

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
