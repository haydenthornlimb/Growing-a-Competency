# Student Assignment Tracker Requirements

## Purpose
Define the expected behavior of a proposed application that helps a student organize assignments and track deadlines. These requirements describe planned functionality; the application has not yet been implemented.

## Functional Requirements

### R1 Add an Assignment
The student can create an assignment with a title, course, due date, and optional notes.

Acceptance criteria:
- A title, course, and valid due date are required.
- Missing required information produces a clear error message.
- A successfully added assignment appears in the assignment list.

### R2 Update an Assignment
The student can edit an existing assignment.

Acceptance criteria:
- The student can change the title, course, due date, or notes.
- Saved changes appear in the assignment list.
- Canceling an edit preserves the previous information.

### R3 Complete an Assignment
The student can mark an assignment complete or return it to incomplete.

Acceptance criteria:
- A new assignment starts as incomplete.
- Marking an assignment complete changes its displayed status.
- Marking it incomplete makes it appear in the incomplete assignment view again.

### R4 Sort Upcoming Work
The student can view incomplete assignments in order of due date.

Acceptance criteria:
- Assignments with earlier due dates appear before later ones.
- Assignments with the same due date are sorted alphabetically by title.
- Completed assignments are excluded from this view.

### R5 Filter by Course
The student can display assignments for a selected course.

Acceptance criteria:
- Selecting a course shows only assignments belonging to that course.
- Selecting All Courses restores the full list.
- A clear message appears when no assignments match the selected course.

### R6 Identify Overdue Work
The application identifies incomplete assignments whose due dates have passed.

Acceptance criteria:
- An incomplete assignment is overdue when its due date is earlier than today's date.
- An assignment due today is not marked overdue.
- Completed assignments are not marked overdue.

### R7 Delete an Assignment
The student can remove an assignment that is no longer needed.

Acceptance criteria:
- The application requests confirmation before deletion.
- Confirming removes the assignment from the list.
- Canceling preserves the assignment.

## Data Requirements
Each assignment will have:
- A unique identifier.
- A title.
- A course.
- A due date.
- Optional notes.
- A completion status.

## Initial Scope
The first version supports one student entering assignments manually. Shared accounts, course website integration, and notifications are outside the initial scope.

## Example Acceptance Check
Create two incomplete assignments with different due dates. Confirm that the earlier assignment appears first. Mark that assignment complete and verify that it disappears from the incomplete assignment view.
