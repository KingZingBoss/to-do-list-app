# To-Do List Application

This project is a simple, interactive To-Do List application built using HTML, CSS, and JavaScript. It allows users to add tasks, mark them as completed, and remove them. The application also saves tasks in the browser's local storage, so they persist even after the page is refreshed.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Add Tasks:** Users can add new tasks to their to-do list.
- **Mark as Completed:** Users can mark tasks as completed, which will apply a line-through style and reduce the opacity.
- **Delete Tasks:** Users can remove tasks from their list.
- **Filter Tasks:** Users can filter tasks by their status: All, Completed, or Incomplete.
- **Persistent Storage:** Tasks are stored in the browser's local storage, so they remain even after a page refresh.

## Technologies Used

- **HTML5:** For structuring the content.
- **CSS3:** For styling the application.
- **JavaScript (ES6+):** For adding interactivity and handling logic.
- **Google Fonts:** For the Poppins font used in the application.
- **Font Awesome & Boxicons:** For icons used in buttons and UI elements.

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

- **Adding a Task:** Enter a task in the input field and click the plus button to add it to your list.
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
