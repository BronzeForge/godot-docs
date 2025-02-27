:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualScriptYieldSignal.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualScriptYieldSignal:

VisualScriptYieldSignal
=======================

**Inherits:** :ref:`VisualScriptNode<class_VisualScriptNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

A Visual Script node yielding for a signal.

Description
-----------

``VisualScriptYieldSignal`` will pause the function execution until the provided signal is emitted.

Properties
----------

+--------------------------------------------------------+--------------------------------------------------------------------+---------------+
| :ref:`StringName<class_StringName>`                    | :ref:`base_type<class_VisualScriptYieldSignal_property_base_type>` | ``&"Object"`` |
+--------------------------------------------------------+--------------------------------------------------------------------+---------------+
| :ref:`CallMode<enum_VisualScriptYieldSignal_CallMode>` | :ref:`call_mode<class_VisualScriptYieldSignal_property_call_mode>` | ``0``         |
+--------------------------------------------------------+--------------------------------------------------------------------+---------------+
| :ref:`NodePath<class_NodePath>`                        | :ref:`node_path<class_VisualScriptYieldSignal_property_node_path>` |               |
+--------------------------------------------------------+--------------------------------------------------------------------+---------------+
| :ref:`StringName<class_StringName>`                    | :ref:`signal<class_VisualScriptYieldSignal_property_signal>`       | ``&""``       |
+--------------------------------------------------------+--------------------------------------------------------------------+---------------+

Enumerations
------------

.. _enum_VisualScriptYieldSignal_CallMode:

.. _class_VisualScriptYieldSignal_constant_CALL_MODE_SELF:

.. _class_VisualScriptYieldSignal_constant_CALL_MODE_NODE_PATH:

.. _class_VisualScriptYieldSignal_constant_CALL_MODE_INSTANCE:

enum **CallMode**:

- **CALL_MODE_SELF** = **0** --- A signal from this :ref:`Object<class_Object>` will be used.

- **CALL_MODE_NODE_PATH** = **1** --- A signal from the given :ref:`Node<class_Node>` in the scene tree will be used.

- **CALL_MODE_INSTANCE** = **2** --- A signal from an instanced node with the given type will be used.

Property Descriptions
---------------------

.. _class_VisualScriptYieldSignal_property_base_type:

- :ref:`StringName<class_StringName>` **base_type**

+-----------+----------------------+
| *Default* | ``&"Object"``        |
+-----------+----------------------+
| *Setter*  | set_base_type(value) |
+-----------+----------------------+
| *Getter*  | get_base_type()      |
+-----------+----------------------+

The base type to be used when :ref:`call_mode<class_VisualScriptYieldSignal_property_call_mode>` is set to :ref:`CALL_MODE_INSTANCE<class_VisualScriptYieldSignal_constant_CALL_MODE_INSTANCE>`.

----

.. _class_VisualScriptYieldSignal_property_call_mode:

- :ref:`CallMode<enum_VisualScriptYieldSignal_CallMode>` **call_mode**

+-----------+----------------------+
| *Default* | ``0``                |
+-----------+----------------------+
| *Setter*  | set_call_mode(value) |
+-----------+----------------------+
| *Getter*  | get_call_mode()      |
+-----------+----------------------+

``call_mode`` determines the target object to wait for the signal emission. See :ref:`CallMode<enum_VisualScriptYieldSignal_CallMode>` for options.

----

.. _class_VisualScriptYieldSignal_property_node_path:

- :ref:`NodePath<class_NodePath>` **node_path**

+----------+----------------------+
| *Setter* | set_base_path(value) |
+----------+----------------------+
| *Getter* | get_base_path()      |
+----------+----------------------+

The node path to use when :ref:`call_mode<class_VisualScriptYieldSignal_property_call_mode>` is set to :ref:`CALL_MODE_NODE_PATH<class_VisualScriptYieldSignal_constant_CALL_MODE_NODE_PATH>`.

----

.. _class_VisualScriptYieldSignal_property_signal:

- :ref:`StringName<class_StringName>` **signal**

+-----------+-------------------+
| *Default* | ``&""``           |
+-----------+-------------------+
| *Setter*  | set_signal(value) |
+-----------+-------------------+
| *Getter*  | get_signal()      |
+-----------+-------------------+

The signal name to be waited for.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
