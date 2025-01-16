# Task Management App

This project is a simple task management application built using **React.js**, **Express.js**, and **MongoDB**. It demonstrates basic CRUD (Create, Read, Update, Delete) operations for managing tasks and includes both front-end and back-end components.

---

## Features

- Add new tasks with a title and description.
- View a list of all tasks.
- Update the status of tasks ("To Do", "In Progress", "Completed").
- Delete tasks.

---

## Project Structure

The application consists of two main components:

### 1. **Backend**
- **Framework**: Express.js
- **Database**: MongoDB

The backend is responsible for handling API requests and performing CRUD operations on the MongoDB database.

### 2. **Frontend**
- **Framework**: React.js

The frontend provides a user-friendly interface to interact with the task management system.

---

## Prerequisites

To run this project, ensure you have the following installed on your system:

- Node.js (v16 or later)
- MongoDB (local or cloud instance)
- npm or yarn

---

## Installation and Setup

### 1. **Clone the Repository**

```bash
git clone https://github.com/your-repo/task-management-app.git
cd task-management-app
```

### 2. **Setup Backend**

Navigate to the backend directory and follow these steps:

1. Install dependencies:
   ```bash
   npm install
   ```

2. Create a `.env` file in the root of the backend folder and set your MongoDB connection string:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   PORT=3000
   ```

3. Start the server:
   ```bash
   npm start
   ```

The backend server will start on `http://localhost:3000`.

### 3. **Setup Frontend**

Navigate to the frontend directory and follow these steps:

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server:
   ```bash
   npm run dev
   ```

The frontend will start on `http://localhost:5173`.

---

## Backend Details

### Routes

- **Add Task**: `POST /add-task`
- **Get All Tasks**: `GET /tasks`
- **Update Task Status**: `PATCH /update-status/:id`
- **Delete Task**: `DELETE /delete-task/:id`

### Dependencies

- `express`
- `mongoose`
- `dotenv`
- `cors`

---

## Frontend Details

### Features

- **Task List**: Displays a list of tasks with their status.
- **Task Form**: Allows users to add new tasks.
- **Task Actions**: Buttons to start, complete, or delete tasks.

### Dependencies

- `react`
- `react-dom`
- `react-redux`
- `@reduxjs/toolkit`
- `formik`
- `yup`
- `react-icons`
- `react-bootstrap`
- `bootstrap`
- `react-hot-toast`

---

## Database

The project uses **MongoDB** for storing task data. Each task document contains the following fields:

- `title` (String, required): The title of the task.
- `description` (String, required): A brief description of the task.
- `status` (String, default: `todo`): The current status of the task (`todo`, `progress`, `completed`).
- `createdAt` (Date, default: current date): The creation date of the task.

---

## Usage

1. Open the frontend application in your browser (`http://localhost:5173`).
2. Add tasks using the form.
3. View the task list and perform actions (update status or delete tasks).

---

## Future Improvements

- Add user authentication.
- Enhance the UI with more advanced styling.
- Implement pagination for tasks.
- Add a search/filter feature.

---

## License

This project is licensed under the MIT License.

