===========================================
Activity Popover depending on Activity Type
===========================================

Manage which popover to display when clicked ``'Mark Done'`` on
activity.

Configuration
=============

For this feature to work, module :code:`mail_activity_popover_toggle`
must be installed and *Hide Popover* enabled/disabled on activity type.

.. image:: media/activity_popover_toggle_conf.png
    :align: center

Mark Done Popover
=================

As standard, there are two available popovers to use when marking
activity as done:

* smaller feedback popover:

.. image:: media/activity_popover_toggle_feedback_chatter.png
    :align: center

.. image:: media/activity_popover_toggle_feedback_kanban.png
    :align: center

* bigger universal (used for multiple purposes) popover:

.. image:: media/activity_popover_toggle_big.png
    :align: center

When *Hide Popover* is enabled on activity type - bigger popover will
be showed instead of the smaller one, when marking activity, with such
activity type, as done.

.. note::
    You can mark activity as done via chatter or kanban view, e.g.:

    .. image:: media/activity_popover_toggle_mark_done_chatter.png
        :align: center

    .. image:: media/activity_popover_toggle_mark_done_kanban.png
        :align: center
