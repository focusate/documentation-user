===========================================================
Confirmation on sending out messages to external recipients
===========================================================

Adding extra confirmation step while sending emails to external 
recipients (partners, followers). This is included in the chatter 
and advanced mail message composition wizard. Confirmation popover 
will appear if email is going to be sent to any of external partners 
with a list of external recipients.

Configuration
=============

To start using this new functionality, module :code:`mail_external_confirm`
must be installed.

Feature can be enabled/disabled in General Settings 
(:menuselection:`Settings --> General Settings --> Discuss`), Discuss 
section by changing value of parameter 'Confirm External Emails':

.. image:: media/mail_external_confirm_enable.png
    :align: center

Functionality
=============

This feature warns the user, that the message he/she is intended to send 
contains any type of external recipients (external partners, portal users). 
It works in *Send Message*, *Log Note* with @ (mention contact) or # (mention 
channel). 

This feature will work on all objects that have mail chatter implemented, 
e.g. Leads & Opportunities, Partners, Sales, Invoices and other Odoo objects.

Add external followers of the lead, opportunity or partner:

.. image:: media/mail_external_confirm_followers.png
    :align: center

Try sending message and you will get a pop-up to confirm sending 
with listed all external recipients names:

.. image:: media/mail_external_confirm_popup.png
    :align: center

.. note::
    Confirmation in pop-up by default will have *Cancel* selection.

Full mail composer has the same functionality as described above.

Channel with external recipients will be triggered, when in channel 
configuration *Send messages by email* is marked:

.. image:: media/mail_external_confirm_channel.png
    :align: center

.. note::
    Please note, that this functionality has no any impact on mass 
    mailing function.