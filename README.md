# To-Do List Application

This project is a simple, interactive To-Do List application built using HTML, CSS, and JavaScript. It allows users to add tasks, mark them as completed, delete tasks, and filter tasks based on their status. The application also stores tasks in the browser's local storage, ensuring they persist even after a page refresh.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [How the App Works](#how-the-app-works)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Add Tasks:** Users can add new tasks to their to-do list.
- **Mark as Completed:** Users can mark tasks as completed, which applies a line-through style and reduces opacity.
- **Delete Tasks:** Users can remove tasks from their list.
- **Filter Tasks:** Users can filter tasks by their status: All, Completed, or Incomplete.
- **Persistent Storage:** Tasks are stored in the browser's local storage, so they remain even after a page refresh.

## Technologies Used

- **HTML5:** For structuring the content.
- **CSS3:** For styling the application.
- **JavaScript (ES6+):** For adding interactivity and handling logic.
- **Google Fonts:** For the Poppins font used in the application.
- **Font Awesome & Boxicons:** For icons used in buttons and UI elements.

## How the App Works

### 1. **Adding a Task**

When the user enters a task in the input field and clicks the plus button (or presses Enter), the `addTodo` function is triggered. This function creates a new `<div>` element with the class `todo`, which contains:
- A `<li>` element that displays the task text.
- A complete button with a checkmark icon.
- A delete button with a trash icon.

The new task is then added to the `<ul>` element with the class `todo-list`. Additionally, the task is saved in the browser's local storage using the `saveLocalTodos` function.

### 2. **Marking a Task as Completed**

When the user clicks the complete button next to a task, the `deleteCheck` function is triggered. This function checks the class of the clicked item. If it's a complete button, the function toggles the `completed` class on the parent `<div>` element, which strikes through the task and reduces its opacity, indicating it's completed.

### 3. **Deleting a Task**

If the user clicks the delete button, the `deleteCheck` function adds a sliding animation class (`slide`) to the parent `<div>`. Once the animation ends, the task is removed from the DOM. Simultaneously, the task is also removed from the local storage using the `removeLocalTodos` function.

### 4. **Filtering Tasks**

The filter dropdown menu allows users to filter tasks based on their status (All, Completed, or Incomplete). The `filterTodo` function is triggered whenever the filter option changes. It loops through all tasks and displays them based on the selected filter option.

### 5. **Persistent Storage**

Tasks are stored in the browser's local storage. The `saveLocalTodos` function is used to store tasks when they are added. The `getLocalTodos` function loads these tasks from local storage when the page is loaded, ensuring that tasks persist across sessions.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/KingZingBoss/todo-list.git
   ```

2. Navigate to the project directory:

   ```bash
   cd todo-list
   ```

3. Open the `index.html` file in your preferred web browser:

   ```bash
   open index.html
   ```

## Usage

- **Adding a Task:** Enter a task in the input field and click the plus button or press Enter to add it to your list.
- **Marking as Completed:** Click the checkmark button next to a task to mark it as completed.
- **Deleting a Task:** Click the trash icon next to a task to delete it.
- **Filtering Tasks:** Use the dropdown menu to filter tasks by their status: All, Completed, or Incomplete.

## Project Structure

```
├── assets
│   ├── css
│   │   └── style.css      # Contains all the styles for the application
│   └── js
│       └── script.js      # Contains the JavaScript logic for the application
├── index.html              # The main HTML file
└── README.md               # Project documentation
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
