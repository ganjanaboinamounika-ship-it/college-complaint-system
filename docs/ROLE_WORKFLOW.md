# Role workflow

### Student
1. Login as Student.
2. Click **Raise a complaint**.
3. Enter title, category, severity and description.
4. Submit.
5. Track Open → In review → Resolved.
6. Read the Dean's solution, root cause and preventive action.

### College Dean
1. Login as College Dean.
2. Open the complaint inbox.
3. Review the student's problem.
4. Select In review or Resolved.
5. Enter the solution/Dean response.
6. Enter root cause.
7. Enter preventive action.
8. Click **Send solution to student**.

The API also blocks `POST /api/complaints` for Dean accounts, so a Dean cannot create a complaint by using the frontend or by manually calling the endpoint.
