# Student Enrollment Form

## Description
This project provides a web-based form for managing student enrollment in a school database. The form allows users to add, update, and reset student records. It interacts with a JSON-based database using JsonPowerDB, ensuring efficient and flexible data management.

## Benefits of Using JsonPowerDB
- **High Performance**: JsonPowerDB provides fast query execution due to its in-memory data storage.
- **Flexible Data Handling**: It supports dynamic data models, which makes it easier to work with varied data structures.
- **Real-time Updates**: Changes in the database are immediately reflected in the application.
- **Simple Integration**: JsonPowerDB offers straightforward integration with web forms and other data interfaces.

## Release History
- **v1.0**: Initial release of the Student Enrollment Form.

## Table of Contents
1. [Description](#description)
2. [Benefits of Using JsonPowerDB](#benefits-of-using-jsonpowerdb)
3. [Release History](#release-history)
4. [Form Implementation](#form-implementation)
5. [Examples of Use](#examples-of-use)
6. [Project Status](#project-status)
7. [Sources](#sources)
8. [Other Information](#other-information)

## Form Implementation

### Student Enrollment Form

**Primary Key**: Roll No.

**Input Fields**:
- Roll-No
- Full-Name
- Class
- Birth-Date
- Address
- Enrollment-Date

**Control Buttons**:
- **Save**: Stores new student records in the database.
- **Update**: Modifies existing student records in the database.
- **Reset**: Clears the form for new data entry.

**Behavior**:
- On page load or control button click, an empty form is displayed with the cursor in the primary key field.
- If the primary key value does not exist in the database:
  - Enable the [Save] and [Reset] buttons.
  - Move the cursor to the next field.
  - Validate that no fields are empty before allowing form submission.
- If the primary key value exists in the database:
  - Display existing data in the form.
  - Enable the [Update] and [Reset] buttons.
  - Keep the primary key field disabled.
  - Allow updates to other fields only after validation.

## Examples of Use
1. **Adding a New Student**:
   - Enter a new Roll-No and complete the other fields.
   - Click [Save] to store the data.

2. **Updating an Existing Student**:
   - Enter an existing Roll-No to retrieve current data.
   - Modify the required fields.
   - Click [Update] to save changes.

3. **Resetting the Form**:
   - Click [Reset] to clear all fields and start afresh.

## Project Status
- **In Progress**: The form implementation is currently being developed.

## Sources
- JsonPowerDB Documentation: [JsonPowerDB Documentation](https://jsonpowerdb.com)

## Other Information
- The form and database integration are implemented using HTML, CSS, and JavaScript.
- Ensure that the JsonPowerDB server is running before using the form.

