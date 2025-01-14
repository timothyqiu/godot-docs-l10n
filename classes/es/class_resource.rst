:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Resource.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Resource:

Resource
========

**Inherits:** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`Animation<class_Animation>`, :ref:`AnimationNode<class_AnimationNode>`, :ref:`AnimationNodeStateMachinePlayback<class_AnimationNodeStateMachinePlayback>`, :ref:`AnimationNodeStateMachineTransition<class_AnimationNodeStateMachineTransition>`, :ref:`AudioBusLayout<class_AudioBusLayout>`, :ref:`AudioEffect<class_AudioEffect>`, :ref:`AudioStream<class_AudioStream>`, :ref:`BakedLightmapData<class_BakedLightmapData>`, :ref:`BitMap<class_BitMap>`, :ref:`ButtonGroup<class_ButtonGroup>`, :ref:`CryptoKey<class_CryptoKey>`, :ref:`CubeMap<class_CubeMap>`, :ref:`Curve<class_Curve>`, :ref:`Curve2D<class_Curve2D>`, :ref:`Curve3D<class_Curve3D>`, :ref:`DynamicFontData<class_DynamicFontData>`, :ref:`EditorSettings<class_EditorSettings>`, :ref:`EditorSpatialGizmoPlugin<class_EditorSpatialGizmoPlugin>`, :ref:`Environment<class_Environment>`, :ref:`Font<class_Font>`, :ref:`GDNativeLibrary<class_GDNativeLibrary>`, :ref:`GIProbeData<class_GIProbeData>`, :ref:`GLTFAccessor<class_GLTFAccessor>`, :ref:`GLTFAnimation<class_GLTFAnimation>`, :ref:`GLTFBufferView<class_GLTFBufferView>`, :ref:`GLTFCamera<class_GLTFCamera>`, :ref:`GLTFDocument<class_GLTFDocument>`, :ref:`GLTFLight<class_GLTFLight>`, :ref:`GLTFMesh<class_GLTFMesh>`, :ref:`GLTFNode<class_GLTFNode>`, :ref:`GLTFSkeleton<class_GLTFSkeleton>`, :ref:`GLTFSkin<class_GLTFSkin>`, :ref:`GLTFSpecGloss<class_GLTFSpecGloss>`, :ref:`GLTFState<class_GLTFState>`, :ref:`GLTFTexture<class_GLTFTexture>`, :ref:`Gradient<class_Gradient>`, :ref:`Image<class_Image>`, :ref:`InputEvent<class_InputEvent>`, :ref:`Material<class_Material>`, :ref:`Mesh<class_Mesh>`, :ref:`MeshLibrary<class_MeshLibrary>`, :ref:`MultiMesh<class_MultiMesh>`, :ref:`NavigationMesh<class_NavigationMesh>`, :ref:`NavigationPolygon<class_NavigationPolygon>`, :ref:`OccluderPolygon2D<class_OccluderPolygon2D>`, :ref:`OccluderShape<class_OccluderShape>`, :ref:`OpenSimplexNoise<class_OpenSimplexNoise>`, :ref:`PackedDataContainer<class_PackedDataContainer>`, :ref:`PackedScene<class_PackedScene>`, :ref:`PhysicsMaterial<class_PhysicsMaterial>`, :ref:`PolygonPathFinder<class_PolygonPathFinder>`, :ref:`RichTextEffect<class_RichTextEffect>`, :ref:`Script<class_Script>`, :ref:`Shader<class_Shader>`, :ref:`Shape<class_Shape>`, :ref:`Shape2D<class_Shape2D>`, :ref:`ShortCut<class_ShortCut>`, :ref:`Skin<class_Skin>`, :ref:`Sky<class_Sky>`, :ref:`SpriteFrames<class_SpriteFrames>`, :ref:`StyleBox<class_StyleBox>`, :ref:`TextFile<class_TextFile>`, :ref:`Texture<class_Texture>`, :ref:`TextureLayered<class_TextureLayered>`, :ref:`Theme<class_Theme>`, :ref:`TileSet<class_TileSet>`, :ref:`Translation<class_Translation>`, :ref:`VideoStream<class_VideoStream>`, :ref:`VisualScriptNode<class_VisualScriptNode>`, :ref:`VisualShaderNode<class_VisualShaderNode>`, :ref:`World<class_World>`, :ref:`World2D<class_World2D>`, :ref:`X509Certificate<class_X509Certificate>`

Clase base para todos los recursos.

Descripción
----------------------

Resource is the base class for all Godot-specific resource types, serving primarily as data containers. Since they inherit from :ref:`Reference<class_Reference>`, resources are reference-counted and freed when no longer in use. They are also cached once loaded from disk, so that any further attempts to load a resource from a given path will return the same reference (all this in contrast to a :ref:`Node<class_Node>`, which is not reference-counted and can be instanced from disk as many times as desired). Resources can be saved externally on disk or bundled into another object, such as a :ref:`Node<class_Node>` or another resource.

\ **Note:** In C#, resources will not be freed instantly after they are no longer in use. Instead, garbage collection will run periodically and will free resources that are no longer in use. This means that unused resources will linger on for a while before being removed.

Tutoriales
--------------------

- :doc:`Resources <../tutorials/scripting/resources>`

- :doc:`When and how to avoid using nodes for everything <../tutorials/best_practices/node_alternatives>`

Propiedades
----------------------

+-----------------------------+---------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`     | :ref:`resource_local_to_scene<class_Resource_property_resource_local_to_scene>` | ``false`` |
+-----------------------------+---------------------------------------------------------------------------------+-----------+
| :ref:`String<class_String>` | :ref:`resource_name<class_Resource_property_resource_name>`                     | ``""``    |
+-----------------------------+---------------------------------------------------------------------------------+-----------+
| :ref:`String<class_String>` | :ref:`resource_path<class_Resource_property_resource_path>`                     | ``""``    |
+-----------------------------+---------------------------------------------------------------------------------+-----------+

Métodos
--------------

+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`_setup_local_to_scene<class_Resource_method__setup_local_to_scene>` **(** **)** |virtual|                  |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| :ref:`Resource<class_Resource>` | :ref:`duplicate<class_Resource_method_duplicate>` **(** :ref:`bool<class_bool>` subresources=false **)** |const| |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`emit_changed<class_Resource_method_emit_changed>` **(** **)**                                              |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| :ref:`Node<class_Node>`         | :ref:`get_local_scene<class_Resource_method_get_local_scene>` **(** **)** |const|                                |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_RID>`           | :ref:`get_rid<class_Resource_method_get_rid>` **(** **)** |const|                                                |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`setup_local_to_scene<class_Resource_method_setup_local_to_scene>` **(** **)**                              |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+
| void                            | :ref:`take_over_path<class_Resource_method_take_over_path>` **(** :ref:`String<class_String>` path **)**         |
+---------------------------------+------------------------------------------------------------------------------------------------------------------+

Señales
--------------

.. _class_Resource_signal_changed:

- **changed** **(** **)**

Emitted whenever the resource changes.

\ **Note:** This signal is not emitted automatically for custom resources, which means that you need to create a setter and emit the signal yourself.

Descripciones de Propiedades
--------------------------------------------------------

.. _class_Resource_property_resource_local_to_scene:

- :ref:`bool<class_bool>` **resource_local_to_scene**

+-----------+---------------------------+
| *Default* | ``false``                 |
+-----------+---------------------------+
| *Setter*  | set_local_to_scene(value) |
+-----------+---------------------------+
| *Getter*  | is_local_to_scene()       |
+-----------+---------------------------+

Si ``true``, el recurso se hará único en cada instancia de su escena local. Por lo tanto, puede modificarse en una instancia de la escena sin afectar a otras instancias de la misma escena.

----

.. _class_Resource_property_resource_name:

- :ref:`String<class_String>` **resource_name**

+-----------+-----------------+
| *Default* | ``""``          |
+-----------+-----------------+
| *Setter*  | set_name(value) |
+-----------+-----------------+
| *Getter*  | get_name()      |
+-----------+-----------------+

The name of the resource. This is an optional identifier. If :ref:`resource_name<class_Resource_property_resource_name>` is not empty, its value will be displayed to represent the current resource in the editor inspector. For built-in scripts, the :ref:`resource_name<class_Resource_property_resource_name>` will be displayed as the tab name in the script editor.

----

.. _class_Resource_property_resource_path:

- :ref:`String<class_String>` **resource_path**

+-----------+-----------------+
| *Default* | ``""``          |
+-----------+-----------------+
| *Setter*  | set_path(value) |
+-----------+-----------------+
| *Getter*  | get_path()      |
+-----------+-----------------+

El camino hacia el recurso. En caso de que tenga su propio archivo, devolverá su ruta de acceso. Si está ligado a la escena, devolverá la ruta de la escena, seguida por el índice del recurso.

Descripciones de Métodos
------------------------------------------------

.. _class_Resource_method__setup_local_to_scene:

- void **_setup_local_to_scene** **(** **)** |virtual|

Función virtual que puede ser sobreescrita para personalizar el valor de comportamiento de :ref:`setup_local_to_scene<class_Resource_method_setup_local_to_scene>`.

----

.. _class_Resource_method_duplicate:

- :ref:`Resource<class_Resource>` **duplicate** **(** :ref:`bool<class_bool>` subresources=false **)** |const|

Duplicates the resource, returning a new resource with the exported members copied. **Note:** To duplicate the resource the constructor is called without arguments. This method will error when the constructor doesn't have default values.

By default, sub-resources are shared between resource copies for efficiency. This can be changed by passing ``true`` to the ``subresources`` argument which will copy the subresources.

\ **Note:** If ``subresources`` is ``true``, this method will only perform a shallow copy. Nested resources within subresources will not be duplicated and will still be shared.

\ **Note:** When duplicating a resource, only ``export``\ ed properties are copied. Other properties will be set to their default value in the new resource.

----

.. _class_Resource_method_emit_changed:

- void **emit_changed** **(** **)**

Emits the :ref:`changed<class_Resource_signal_changed>` signal.

If external objects which depend on this resource should be updated, this method must be called manually whenever the state of this resource has changed (such as modification of properties).

The method is equivalent to:

::

    emit_signal("changed")

\ **Note:** This method is called automatically for built-in resources.

----

.. _class_Resource_method_get_local_scene:

- :ref:`Node<class_Node>` **get_local_scene** **(** **)** |const|

Si :ref:`resource_local_to_scene<class_Resource_property_resource_local_to_scene>` está activado y el recurso se cargó desde una instanciación :ref:`PackedScene<class_PackedScene>`, devuelve la escena local en la que se utiliza la copia única de este recurso. En caso contrario, devuelve ``null``.

----

.. _class_Resource_method_get_rid:

- :ref:`RID<class_RID>` **get_rid** **(** **)** |const|

Returns the RID of the resource (or an empty RID). Many resources (such as :ref:`Texture<class_Texture>`, :ref:`Mesh<class_Mesh>`, etc) are high-level abstractions of resources stored in a server, so this function will return the original RID.

----

.. _class_Resource_method_setup_local_to_scene:

- void **setup_local_to_scene** **(** **)**

Este método se llama cuando un recurso con :ref:`resource_local_to_scene<class_Resource_property_resource_local_to_scene>` activado se carga desde una instanciación :ref:`PackedScene<class_PackedScene>`. Su comportamiento puede ser personalizado anulando :ref:`_setup_local_to_scene<class_Resource_method__setup_local_to_scene>` desde el script.

Para la mayoría de los recursos, este método no realiza ninguna lógica de base. :ref:`ViewportTexture<class_ViewportTexture>` realiza una lógica personalizada para establecer correctamente la textura del proxy y las banderas en el viewport local.

----

.. _class_Resource_method_take_over_path:

- void **take_over_path** **(** :ref:`String<class_String>` path **)**

Establece la ruta del recurso, anulando potencialmente una entrada de caché existente para esta ruta. Esto difiere del establecimiento de :ref:`resource_path<class_Resource_property_resource_path>`, ya que este último daría un error si otro recurso ya estuviera en caché para la ruta dada.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
