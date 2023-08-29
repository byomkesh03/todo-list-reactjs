# To-Do List App Documentation

This documentation provides an overview of the "To-Do List" app created using React. The app allows users to add tasks to a list, delete tasks, and persists task data using local storage.

## Table of Contents

- [Features](#features)
- [Component Structure](#component-structure)
- [Local Storage](#local-storage)
- [Styling](#styling)

## Features

1. **Adding Tasks**: Users can enter a new task in the input field and click the "Add Task" button to add it to the list.
2. **Deleting Tasks**: Each task in the list is accompanied by a "Delete" button. Clicking this button removes the corresponding task from the list.
3. **Local Storage**: Task data is persisted using local storage, ensuring that tasks are retained even after the user closes or refreshes the page.

## Component Structure

The app is structured using two main components:

1. **`App` Component**:
   - Manages the state of tasks and the new task input.
   - Utilizes the `useEffect` hook to load and save tasks to local storage.
   - Renders the input field, "Add Task" button, and the list of tasks.

2. **`Task` Component**:
   - Accepts `task` and `onDelete` as props.
   - Renders an individual task along with a "Delete" button.
   - Calls the `onDelete` function when the "Delete" button is clicked.

## Local Storage

Local storage is used to store and retrieve task data between sessions. The `useEffect` hook is used to manage the interaction with local storage. Tasks are loaded from local storage when the app initially loads, and they are saved to local storage whenever the tasks state changes.

## Styling

Styling for the app is done using CSS. The app is centered on the page, and tasks are displayed in a list format. Each task has a border at the bottom and is accompanied by a "Delete" button for removal.

## How to Run the App

1. Ensure you have Node.js and npm installed.
2. Clone the repository or create a new React app using `npx create-react-app todo-list-app`.
3. Replace the content of `src/App.js` with the code provided in the documentation.
4. Update the `src/Task.js` and `src/App.css` files as instructed.
5. Run the app using `npm start`.
6. Access the app in your browser at http://localhost:3000.


