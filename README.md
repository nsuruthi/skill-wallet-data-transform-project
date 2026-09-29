Source Data Upload & Staging Table Creation

Uploaded the source spreadsheet containing 100 employee records into ServiceNow using the Load Data module.

Created a temporary import staging table named u_employee_staging to hold the raw uploaded data.

Transform Map Configuration & Field Mapping

Created a new Table Transform Map named Employee Data Transform Map targeting the standard ServiceNow User (sys_user) table.

Utilized Auto Map Matching Fields to map staging attributes (such as name, department, location, phone, and active status) to target fields on the sys_user table.

Coalesce & Data Transformation Execution
Configured u_email as the Coalesce field (Coalesce = true) to serve as the unique identifier, preventing duplicate user records.

Executed the transform map, resulting in 100 records inserted into sys_user with 0 errors.

Report & Dashboard Creation

Navigated to Reports > Create New to generate visual reports analyzing the newly imported dataset (e.g., employee distribution by department and active status).

Built a custom ServiceNow Dashboard (pa_dashboards) and added the report widgets to provide real-time data visibility and administrative analytics.
Validation & Project Submission



Verified the transformed records directly in the sys_user.list view.


Uploaded the project evidence, GitHub repository URL, and demo link to the SkillWallet portal for final mentor review.
