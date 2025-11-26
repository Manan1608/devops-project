Q2 – SDLC Report
Project: To-Do List Application
SDLC Model Used: Waterfall

1. Introduction
This document describes the design of a simple To-Do List Application using the Waterfall Software Development Life Cycle model. The goal of the application is to help users create, update, and manage daily tasks. The Waterfall model is suitable because the requirements are simple, defined, and unlikely to change.

2. Requirements Document

Functional Requirements:
- Users can create a new task.
- Users can edit existing tasks.
- Users can delete tasks.
- Users can mark tasks as completed.
- Users can view all tasks in a list.
- Completed tasks should be displayed separately or highlighted.

Non-Functional Requirements:
- The interface should be simple and user-friendly.
- Fast loading and quick response time.
- Data should be stored securely (local storage or small database).
- The app should work on both desktop and mobile.
- Low memory usage and smooth functionality.

3. Why Waterfall Model is Suitable
The Waterfall model is linear and easy to follow, making it ideal for beginners and academic projects. Requirements for this project are stable and well-defined. The model allows clear documentation of each phase and reduces confusion. It is low-risk and best suited for small projects like a To-Do List application.

4. SDLC Phases (Waterfall Model)

4.1 Requirements Phase
All system requirements were listed, including the essential features such as adding, editing, deleting, and marking tasks as completed. The project is small, so requirements are easy to understand.

4.2 Design Phase

a) Architecture Design:
The application follows a simple three-layer architecture:
1. User Interface – screens to add, edit, and view tasks
2. Application Logic – processing add/edit/delete operations
3. Storage Layer – LocalStorage, JSON file, or SQLite

b) UI Design:
- Home page showing the list of tasks
- Add task screen or pop-up
- Edit task screen
- Completed tasks section

c) Database Design:
Fields:
id – unique task ID
title – task name
description – optional details
status – completed or not completed
created_at – timestamp

4.3 Implementation Phase (Planned Only)
The app would be built using HTML, CSS, and JavaScript. Data would be stored using LocalStorage or a JSON file. Planned modules include:
- Add Task Module
- Edit Task Module
- Delete Task Module
- Mark as Completed Module
- Task Display Module

4.4 Testing Phase
Sample Test Cases:

Test Case: Add Task
Input: "Buy groceries"
Expected Output: Task appears in the list.

Test Case: Edit Task
Input: Change task name
Expected Output: Edited task is displayed correctly.

Test Case: Delete Task
Input: Click delete button
Expected Output: Task is removed from the list.

Test Case: Complete Task
Input: Click checkbox
Expected Output: Task is marked completed and styled accordingly.

4.5 Deployment Phase
The app can be deployed on GitHub Pages, Netlify, or any basic hosting platform. Only static files are required, making deployment simple.

5. Conflict Resolution Process
Requirement conflicts are resolved through discussion and documentation. Git and GitHub help avoid version conflicts by keeping track of changes. Team members can review and merge changes effectively. Misunderstandings are fixed by choosing the simplest, most appropriate option.

6. Key Lessons Learned
- SDLC helps structure the development process.
- Waterfall is ideal for small, well-defined projects.
- Requirement clarity reduces development mistakes.
- UI and database planning make implementation easier.
- Testing ensures reliability of the app’s features.
- Documentation is important even without coding.
