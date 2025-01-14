:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the StreamPeerTCP.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_StreamPeerTCP:

StreamPeerTCP
=============

**Inherits:** :ref:`StreamPeer<class_StreamPeer>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

TCP stream peer.

Descripción
----------------------

TCP stream peer. Este objeto puede ser utilizado para conectarse a servidores TCP, o también es devuelto por un servidor TCP.

Métodos
--------------

+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>`    | :ref:`connect_to_host<class_StreamPeerTCP_method_connect_to_host>` **(** :ref:`String<class_String>` host, :ref:`int<class_int>` port **)** |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| void                                     | :ref:`disconnect_from_host<class_StreamPeerTCP_method_disconnect_from_host>` **(** **)**                                                    |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`              | :ref:`get_connected_host<class_StreamPeerTCP_method_get_connected_host>` **(** **)** |const|                                                |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                    | :ref:`get_connected_port<class_StreamPeerTCP_method_get_connected_port>` **(** **)** |const|                                                |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Status<enum_StreamPeerTCP_Status>` | :ref:`get_status<class_StreamPeerTCP_method_get_status>` **(** **)**                                                                        |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                  | :ref:`is_connected_to_host<class_StreamPeerTCP_method_is_connected_to_host>` **(** **)** |const|                                            |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+
| void                                     | :ref:`set_no_delay<class_StreamPeerTCP_method_set_no_delay>` **(** :ref:`bool<class_bool>` enabled **)**                                    |
+------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------+

Enumeraciones
--------------------------

.. _enum_StreamPeerTCP_Status:

.. _class_StreamPeerTCP_constant_STATUS_NONE:

.. _class_StreamPeerTCP_constant_STATUS_CONNECTING:

.. _class_StreamPeerTCP_constant_STATUS_CONNECTED:

.. _class_StreamPeerTCP_constant_STATUS_ERROR:

enum **Status**:

- **STATUS_NONE** = **0** --- El estado inicial del ``StreamPeerTCP``. Este es también el estado después de la desconexión.

- **STATUS_CONNECTING** = **1** --- Un estado que representa un ``StreamPeerTCP`` que se está conectando a un host.

- **STATUS_CONNECTED** = **2** --- Un estado que representa un ``StreamPeerTCP`` que está conectado a un host.

- **STATUS_ERROR** = **3** --- Un estado que representa un :ref:`StreamPeerSSL<class_StreamPeerSSL>` en estado de error.

Descripciones de Métodos
------------------------------------------------

.. _class_StreamPeerTCP_method_connect_to_host:

- :ref:`Error<enum_@GlobalScope_Error>` **connect_to_host** **(** :ref:`String<class_String>` host, :ref:`int<class_int>` port **)**

Se conecta al par especificado ``host:port``. Un nombre de host se resolverá si es válido. Devuelve :ref:`@GlobalScope.OK<class_@GlobalScope_constant_OK>` en caso de éxito o :ref:`@GlobalScope.FAILED<class_@GlobalScope_constant_FAILED>` en caso de fracaso.

----

.. _class_StreamPeerTCP_method_disconnect_from_host:

- void **disconnect_from_host** **(** **)**

Se desconecta del host.

----

.. _class_StreamPeerTCP_method_get_connected_host:

- :ref:`String<class_String>` **get_connected_host** **(** **)** |const|

Devuelve la IP de este par.

----

.. _class_StreamPeerTCP_method_get_connected_port:

- :ref:`int<class_int>` **get_connected_port** **(** **)** |const|

Devuelve el puerto de este par.

----

.. _class_StreamPeerTCP_method_get_status:

- :ref:`Status<enum_StreamPeerTCP_Status>` **get_status** **(** **)**

Devuelve el estado de la conexión, ver :ref:`Status<enum_StreamPeerTCP_Status>`.

----

.. _class_StreamPeerTCP_method_is_connected_to_host:

- :ref:`bool<class_bool>` **is_connected_to_host** **(** **)** |const|

Returns ``true`` if this peer is currently connected or is connecting to a host, ``false`` otherwise.

----

.. _class_StreamPeerTCP_method_set_no_delay:

- void **set_no_delay** **(** :ref:`bool<class_bool>` enabled **)**

If ``enabled`` is ``true``, packets will be sent immediately. If ``enabled`` is ``false`` (the default), packet transfers will be delayed and combined using `Nagle's algorithm <https://en.wikipedia.org/wiki/Nagle%27s_algorithm>`__.

\ **Note:** It's recommended to leave this disabled for applications that send large packets or need to transfer a lot of data, as enabling this can decrease the total available bandwidth.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
