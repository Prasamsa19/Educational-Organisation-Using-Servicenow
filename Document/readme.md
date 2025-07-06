📘 Educational Organization — ServiceNow Setup Guide
1. Setting Up a ServiceNow Instance
Provision a Developer or PDI instance via the ServiceNow Developer site.

Log in as admin, confirm plugins, roles, and version compatibility.

Optionally use Guided Setup for product configuration 
servicenow.com
.

2. Creating an Update Set
Navigate to System Update Sets → Local Update Sets.

Click New, assign a clear naming pattern (e.g., REQ1234_GLOBAL_v1) and description 
servicenow.com
+4
servicenow.com
+4
servicenow.com
+4
.

Select it as your current update set before any changes.

Tip: Only customizations tied to the active set are captured 
support.servicenow.com
+4
servicenow.com
+4
servicenow.com
+4
servicenow.com
.

3. Creating a Table
Go to System Definition → Tables → New.

Provide Table Label & Name; choose a parent table or extend.

Add fields, types, default values, and indexing as needed.

For scripted creation, use a Script Include with GlideTableCreator 
servicenow.com
+11
servicenow.com
+11
docs.akeyless.io
+11
servicenow.com
.

4. Form Layout
Open a record from your table.

Right-click header and choose Configure → Form Layout.

Drag fields between Available & Selected; organize sections.

Save to capture layout changes in the Update Set 
docs.akeyless.io
+7
servicenow.com
+7
servicenow.com
+7
servicenow.com
+1
docs.akeyless.io
+1
.

5. Form Design
For UI Builder / Service Operations Workspace, go to Configure Page → Form Layout for UI-centric controls 
servicenow.com
.

Adjust tabs, sections, field ordering as required.

6. Number Maintenance
Use System Definition → Number Maintenance to set unique auto_number formats for tables.

Ensure format and counters meet your organizational requirements.

7. Process Flow
Build business logic via Flow Designer or legacy Workflows.

Design approvals, data transformations, and notifications with flows and conditions.

Trigger flows using UI Actions, Business Rules, or Script Actions.

8. Client Script
Navigate to System Definition → Client Scripts.

Choose trigger type (onLoad, onChange, onSubmit, onCellEdit).

Define UI behavior with g_form APIs—e.g. g_form.setVisible(), g_form.addOption().

Use Script Actions combined with Events for server-client tasks 
servicenow.com
+9
docs.akeyless.io
+9
servicenow.com
+9
servicenow.com
+3
servicenow.com
+3
support.servicenow.com
+3
.

Result
By following this guide:

You’ll have a fully functional custom table with a purposeful form layout and numbering scheme.

A process flow will automate user interactions and backend workflows.

Your client scripts will enforce UI logic.


