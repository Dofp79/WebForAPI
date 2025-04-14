# User Management System

This project provides a basic **User Management Interface** using **HTML**, **Bootstrap**, **jQuery**, and **REST API integration**.  
It includes two main modules: a table view to display users, and a form to create or update user data.

---

## Project Structure & Class Responsibilities

### 1. `Start.html`
> **Purpose:** Displays a list of users retrieved from the backend.

- `container`, `row`, `col-*`: Used for responsive layout with Bootstrap Grid.
- `.btn`, `.btn-primary`, `.btn-success`, `.btn-danger`: Styled buttons for actions like *Create*, *Edit*, and *Delete*.
- `.table`, `.table-striped`: Bootstrap classes for clean and alternating row designs.
- JavaScript functions:
  - `View()`: Fetches and populates user data.
  - `GoToFormCreate()`: Navigates to the form page.
  - `Edit` / `Delete`: Handle individual user operations via API.

---

### 2. `Registration.html`
> **Purpose:** Provides a form to create or update a user.

- `form-group`, `form-control`: Bootstrap classes for form styling and spacing.
- `.btn-primary`: Used for the **Save** button.
- `.btn-warning`: Used for the **Back to** button.
- JavaScript functions:
  - `SaveUser()`: Submits user data via POST (create) or PUT (update).
  - `PainUser(id)`: Populates form fields when editing.
  - `$.urlParam()`: Helper function to extract parameters from URL.
