## Company Management Page

The company management page allows users to select a company type, enter a company code description, and manage the active status of the company. Users can add or update company information, clear the form, and view modification details.

### Business Rules
1. When a user selects a company type, the form updates to reflect the selected type.
2. The "Company Code Description" field is mandatory and must not exceed 250 characters.
3. The "Add" button is only rendered if no company type is selected.
4. The "Update" button is only rendered if a company type is selected.
5. The "Last Modified" and "Modified By" fields are only displayed if a company type is selected.
6. The "Clear" button resets the form fields to their default values.

### Field Descriptions

#### Form Control: Company Code

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Company Code                                 |
| Type        | Dropdown                                      |
| Label       | Company Code                                 |
| Display     | Select One Menu                              |
| Visibility  | Enabled                                      |
| Action      | Updates the form based on the selected company type. |
| Constraint  | N/A                                          |

#### Form Control: Company Code Description

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Company Code Description                     |
| Type        | Input                                        |
| Label       | Company Code Description                     |
| Display     | Text Field                                   |
| Visibility  | Enabled                                      |
| Action      | N/A                                          |
| Constraint  | Required, maximum length of 250 characters.  |

#### Form Control: Active

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Active                                       |
| Type        | Checkbox                                     |
| Label       | Active                                       |
| Display     | Boolean Checkbox                             |
| Visibility  | Enabled                                      |
| Action      | N/A                                          |
| Constraint  | N/A                                          |

#### Form Control: Last Modified

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Last Modified                                |
| Type        | Read Only                                    |
| Label       | Last Modified                                |
| Display     | Text Field                                   |
| Visibility  | Visible only if a company type is selected   |
| Action      | N/A                                          |
| Constraint  | Displays the date in "yyyy-MMM-dd" format.   |

#### Form Control: Modified By

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Modified By                                  |
| Type        | Read Only                                    |
| Label       | Modified By                                  |
| Display     | Text Field                                   |
| Visibility  | Visible only if a company type is selected   |
| Action      | N/A                                          |
| Constraint  | N/A                                          |

#### Form Control: Add

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Add                                          |
| Type        | Button                                       |
| Label       | Add                                          |
| Display     | Command Button                               |
| Visibility  | Rendered only if no company type is selected |
| Action      | Executes the add action and updates the form |
| Constraint  | N/A                                          |

#### Form Control: Update

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Update                                       |
| Type        | Button                                       |
| Label       | Update                                       |
| Display     | Command Button                               |
| Visibility  | Rendered only if a company type is selected  |
| Action      | Executes the update action and updates the form |
| Constraint  | N/A                                          |

#### Form Control: Clear

| **Data Entry Form Control**   |                            |
|-------------|----------------------------------------------|
| Name        | Clear                                        |
| Type        | Link                                         |
| Label       | Clear                                        |
| Display     | Command Link                                 |
| Visibility  | Enabled                                      |
| Action      | Clears the form fields and updates the panel |
| Constraint  | N/A                                          |

### Table Column Descriptions

There are no explicit data tables defined within this JSF XHTML file. The page primarily consists of form controls for managing company information.