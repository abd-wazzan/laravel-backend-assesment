# Laravel Backend Assessment

## Task Management System

Your task is to develop the backend API for a task management system. The system should allow users to perform CRUD operations on tasks and provide the functionality to manage tags associated with tasks. Additionally, you need to implement file management, task state logging, and email notifications, and write automated tests for your endpoints.

### Requirements:

**1. Task Management API**

Implement the CRUD operations for tasks, including creating, reading, updating, and deleting tasks.
Each task should have the following attributes:
Name (maximum 55 characters)
Description (maximum 1500 characters)
Deadline (datetime)
Status (pending, in progress, done)
Tasks can have multiple tags associated with them.
The user can choose from the existing tags or create new ones for future tasks. In the list task endpoint, we should show the first 30 chars or the description content.

**2. Tag Management**

Develop functionality to list tags with their respective count of usages to use in task tags selection.
Tags can be used by multiple tasks.
The current database has 10,000 tags.

**3. Authorization and Authentication**

Only administrators should be able to delete tasks.

**4. File Management**

Tasks can have up to 10 files attached.
Each file should be limited to 10KB in size.

**5. Task State Logging**

Implement a mechanism to log the states of tasks as they transition between pending, in progress, and done.
Include the information about who transmitted the task to the new state.

**6. Database**

Create appropriate database migrations for tasks, tags, logs, and files.
Seed the database with 2,000 tasks and 10,000 tags.

**7. API Documentation**

Utilize Laravel Scribe or a similar tool to generate API documentation for the developed endpoints.

**8. Email Notifications**

Send an email notification for each task that has a deadline within the next 30 minutes.

**9. Additional Query**

Write a pure SQL query in the readme file that retrieve all tasks that have a pending status, a deadline within the next 24 hours, and at least two associated tags.


### Submission Guidelines:

Set up a fresh Laravel project.

Create the necessary migrations for tasks, tags, and files.

Seed the database with the dummy data.

Implement the API endpoints for task management, tag listing, and other required functionality.

Generate API documentation using Laravel Scribe or a similar tool.

Write automated tests for your API endpoints.

Test the API endpoints and automated tests thoroughly.

Demonstrate your solution by making a sample request to create a task, retrieve tasks, update a task, delete a task, list tags, and any other relevant endpoints.

Provide clear instructions on how to run and test your code.

### Evaluation Criteria:

Code structure, organization, and adherence to Laravel conventions.

Correctness and completeness of the implemented functionality.

Proper usage of Laravel's built-in features and libraries.

Handling of potential error conditions and edge cases.

Clear and well-documented code.

Efficient database queries and consideration for performance.

Overall code quality and best practices.

Feel free to ask any clarifying questions before you begin the assessment.

**Good luck!**
