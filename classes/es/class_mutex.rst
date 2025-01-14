:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Mutex.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Mutex:

Mutex
=====

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

Un mutex de sincronización (exclusión mutua).

Descripción
----------------------

Un mutex de sincronización (exclusión mutua). Se utiliza para sincronizar múltiples :ref:`Thread<class_Thread>`\ s, y equivale a un :ref:`Semaphore<class_Semaphore>` binario. Garantiza que sólo un hilo puede adquirir el bloqueo a la vez. Un mutex puede utilizarse para proteger una sección crítica; sin embargo, hay que tener cuidado de evitar los bloqueos.

Tutoriales
--------------------

- :doc:`../tutorials/performance/threads/using_multiple_threads`

Métodos
--------------

+---------------------------------------+----------------------------------------------------------+
| void                                  | :ref:`lock<class_Mutex_method_lock>` **(** **)**         |
+---------------------------------------+----------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>` | :ref:`try_lock<class_Mutex_method_try_lock>` **(** **)** |
+---------------------------------------+----------------------------------------------------------+
| void                                  | :ref:`unlock<class_Mutex_method_unlock>` **(** **)**     |
+---------------------------------------+----------------------------------------------------------+

Descripciones de Métodos
------------------------------------------------

.. _class_Mutex_method_lock:

- void **lock** **(** **)**

Locks this ``Mutex``, blocks until it is unlocked by the current owner.

\ **Note:** This function returns without blocking if the thread already has ownership of the mutex.

----

.. _class_Mutex_method_try_lock:

- :ref:`Error<enum_@GlobalScope_Error>` **try_lock** **(** **)**

Tries locking this ``Mutex``, but does not block. Returns :ref:`@GlobalScope.OK<class_@GlobalScope_constant_OK>` on success, :ref:`@GlobalScope.ERR_BUSY<class_@GlobalScope_constant_ERR_BUSY>` otherwise.

\ **Note:** This function returns :ref:`@GlobalScope.OK<class_@GlobalScope_constant_OK>` if the thread already has ownership of the mutex.

----

.. _class_Mutex_method_unlock:

- void **unlock** **(** **)**

Unlocks this ``Mutex``, leaving it to other threads.

\ **Note:** If a thread called :ref:`lock<class_Mutex_method_lock>` or :ref:`try_lock<class_Mutex_method_try_lock>` multiple times while already having ownership of the mutex, it must also call :ref:`unlock<class_Mutex_method_unlock>` the same number of times in order to unlock it correctly.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
