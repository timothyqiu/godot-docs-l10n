:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeVectorDerivativeFunc.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeVectorDerivativeFunc:

VisualShaderNodeVectorDerivativeFunc
====================================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Calcula un derivado vectorial dentro del gráfico shader visual.

Descripción
----------------------

Este nodo sólo está disponible en shader visuales ``Fragment`` y ``Light``.

Propiedades
----------------------

+---------------------------------------------------------------------+-------------------------------------------------------------------------------+-------+
| :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` | :ref:`function<class_VisualShaderNodeVectorDerivativeFunc_property_function>` | ``0`` |
+---------------------------------------------------------------------+-------------------------------------------------------------------------------+-------+

Enumeraciones
--------------------------

.. _enum_VisualShaderNodeVectorDerivativeFunc_Function:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_SUM:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_X:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_Y:

enum **Function**:

- **FUNC_SUM** = **0** --- Suma del derivado absoluto en ``x`` y ``y``.

- **FUNC_X** = **1** --- Derivado en ``x`` utilizando la diferenciación local.

- **FUNC_Y** = **2** --- Derivado en ``y`` utilizando la diferenciación local.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_VisualShaderNodeVectorDerivativeFunc_property_function:

- :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` **function**

+-----------+---------------------+
| *Default* | ``0``               |
+-----------+---------------------+
| *Setter*  | set_function(value) |
+-----------+---------------------+
| *Getter*  | get_function()      |
+-----------+---------------------+

Un tipo de derivado. Véase :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` para las opciones.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
