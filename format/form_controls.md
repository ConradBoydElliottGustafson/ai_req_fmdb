## Customer Management Page

The customer management page allows users to search and find customers, Add new customers, delete customers and edit customers. The field mappings and controls are outlined below

### Business Rules
1.	If a user clicks Add, a new customer ID is generated and the customer is added as an active record (stored in the main DS table).
2.	Whenever a record is inserted into the primary customer table, a new customer ID is generated for that record.
3.	customer ID is persistent throughout the lifetime of the record.
4.	All mandatory fields must be entered.

### Field Descriptions

#### Form Control: Cancel

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Cancel                                       |
| Type        | Input                                        |
| Label       | Cancel                                       |
| Display     | Button                                       |
| Visibility  | Enabled                                      |
| Action      | Resets all fields to their default values.   |
| Constraint  | N/A                                          |

#### Form Control: Submit

| **Data Entry Form Control**   |                                           |
|-------------|-------------------------------------------------------------|
| Name        | Submit                                                      |
| Type        | Input                                                       |
| Label       | Submit                                                      |
| Display     | Button                                                      |
| Visibility  | Enabled                                                     |
| Action      | Saves the record to the customer table as identified below. |
| Constraint  | Only submits if all fields are fulfilled. Otherwise, an error is displayed. |

#### Table Column: Customer Name

| **Table Column**   |         |
|--------------------|---------|
| Name        | Customer Name  |
| Mandatory   | True           |
| Type        | Input          |
| Label       | Name           |
| Display     | Text Field     |
| Visibility  | Visible        |
| Source      | customer.name  |
| Constraint  | N/A            |

#### Table Column: Status

| **Table Column**   |       |
|--------------------|-------|
| Name        | Status       |
| Mandatory   | True         |
| Type        | Read Only    |
| Label       | Status       |
| Display     | Text Field   |
| Visibility  | Not visible  |
| Source      | customer.status      |
| Constraint  | Default to 'ACTIVE'  |