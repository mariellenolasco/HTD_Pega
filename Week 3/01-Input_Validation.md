# Input Validation with Validate and Edit Validate Rules
In Pega, Validate and Edit Validate rules are used to enforce data validation rules within your application. These rules ensure that data entered by users meets certain criteria and is valid according to your business requirements. 

1. **Validate Rules**:
   - **Purpose**: Validate rules are used to validate the entire data entered by a user before it is committed to the database.
   - **Scope**: Validate rules are typically applied at the time of form submission or when a user tries to advance to the next step in a process.
   - **Validation Logic**: Validate rules contain logic to check the validity of one or more properties based on specified conditions. If the data fails validation, an error message is displayed to the user, and the user is prevented from proceeding until the data is corrected.
   - **Example**: A validate rule might check that a customer's email address is in the correct format or that a required field is not empty.

2. **Edit Validate Rules**:
   - **Purpose**: Edit Validate rules are used to validate individual property values as they are entered or modified by a user.
   - **Scope**: Edit Validate rules are applied dynamically as users interact with the application interface, providing real-time feedback on data entry.
   - **Validation Logic**: Edit Validate rules contain logic to check the validity of a single property value based on specified conditions. If the data fails validation, an error message is displayed next to the field being edited, and the user is prompted to correct the data before proceeding.
   - **Example**: An edit validate rule might check that a password meets minimum length and complexity requirements as the user types it into a password field.

When configuring Validate and Edit Validate rules in Pega, you typically define the following elements:

- **Conditions**: Specify the conditions under which the validation logic should be applied.
- **Validation Logic**: Implement the actual validation rules using expressions, functions, or custom Java code.
- **Error Messages**: Define error messages to be displayed to the user if the data fails validation.

To configure Validate and Edit Validate rules in Pega, you can use the Pega Designer Studio or App Studio interface. These rules can be associated with specific properties, fields, or sections within your application to enforce data validation throughout the user interface.

Overall, Validate and Edit Validate rules play a crucial role in ensuring data integrity and user input correctness in Pega applications. They help maintain data quality and consistency by preventing users from entering invalid or incorrect data.