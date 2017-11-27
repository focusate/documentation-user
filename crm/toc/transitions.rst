=================================================
Transition records usage in leads & opportunities
=================================================

Transition record is a record that is created when one of the following
happens:

* Lead is converted to Opportunity.
* Opportunity stage is changed.
* Opportunity is won.
* Opportunity is lost.
* Opportunity goes from lost to active again.

Transition fields and mapping with general terms
================================================

+------------------+------------+-------------------+------------------+-----------------------------------+
| Key              | Type       | Label             |   General Label  |    Description                    |
+==================+============+===================+==================+===================================+
| id               |  integer   |  ID               | ID               | Internal database ID              |
+------------------+------------+-------------------+------------------+-----------------------------------+
| create_date      |  datetime  |  Created On       | Created On       | When transition was created       |
+------------------+------------+-------------------+------------------+-----------------------------------+
| create_uid       |  many2one  |  Created By       | Created By       | Who created transition            |
+------------------+------------+-------------------+------------------+-----------------------------------+
| date_deadline    |  date      |  Expected Closing |                  | When opportunity is expected to   |
|                  |            |                   |                  | be closed.                        |
+------------------+------------+-------------------+------------------+-----------------------------------+
| lead_id          |  many2one  | Lead/Opportunity  | Lead/Opportunity | Relation with lead or opportunity |
+------------------+------------+-------------------+------------------+-----------------------------------+
| name             |  char      | Opportunity Name  | Transformation   | Name name of opportunity          |
+------------------+------------+-------------------+------------------+-----------------------------------+
| user_id          |  many2one  | Salesperson       | Owner            | Responsible user for opportunity  |
+------------------+------------+-------------------+------------------+-----------------------------------+
| team_id          |  many2one  | Sales Channel     | Business Unit    | Sales Channel (Team) for this     |
|                  |            |                   |                  | opportunity.                      |
+------------------+------------+-------------------+------------------+-----------------------------------+
| partner_id       |  many2one  | Customer          | Account          | Customer for this opportunity     |
+------------------+------------+-------------------+------------------+-----------------------------------+
| throughput       |  float     | Throughput        | Throughput       |                                   |
+------------------+------------+-------------------+------------------+-----------------------------------+
| planned_revenue  |  float     | Expected Revenue  | Est. Value       |                                   |
+------------------+------------+-------------------+------------------+-----------------------------------+
| prev_stage_id    |  many2one  | Previous Stage    | Previous Stage   |                                   |
+------------------+------------+-------------------+------------------+-----------------------------------+
| current_stage_id |  many2one  | Next Stage        | Next Stage       |                                   |
+------------------+------------+-------------------+------------------+-----------------------------------+
| lost_reason      |  many2one  | Lost Reason       | Lost Reason      | Identifies if opportunity is lost |
+------------------+------------+-------------------+------------------+-----------------------------------+
| type             |  selection | Type              | Type             | Type of lead/opportunity. Either  |
|                  |            |                   |                  | 'lead' or 'opportunity'.          |
+------------------+------------+-------------------+------------------+-----------------------------------+
| description      |  text      | Notes             | Description      | Information about opportunity.    |
+------------------+------------+-------------------+------------------+-----------------------------------+
