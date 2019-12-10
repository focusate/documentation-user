=================================
Limit Number of Active Activities
=================================

Specify on which models (that use activities) and how many activities
can be active per user per record.


Configuration
=============

For this feature to work, module :code:`mail_activity_limit` must be
installed and *Activity Limit* in Discuss section of General Settings
must be configured. Value of *Activity Limit* must be a dictionary,
where key is model and value is number of allowed active activities per
user per record (e.g. ``{'res.partner': 2, 'crm.lead': 1}`` means, that
user can only have two active activities on the same partner and one -
on the same lead/opportunity).

.. image:: media/activity_limit_conf.png
    :align: center
