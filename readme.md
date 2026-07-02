# Todo Application

A clean, browser-based todo application built with HTML, CSS, JavaScript, and Bootstrap. It helps users add, edit, delete, complete, and restore tasks through a simple dark-themed interface with audio feedback.

## Overview

This repository contains a lightweight frontend todo app that runs directly in the browser. It does not require a backend, database, package manager, or build setup. The application focuses on essential task management actions while keeping the project structure organized and easy to understand.

Users can add tasks, track pending and completed task counts, move tasks between todo and completed sections, edit task text, and confirm before deleting a task.

## Features

- Add new tasks by typing in the input field and pressing Enter.
- Edit existing tasks through a Bootstrap modal.
- Delete tasks with a confirmation modal.
- Mark tasks as complete using a checkbox.
- Move completed tasks into a dedicated completed section.
- Restore completed tasks back to the todo list by unchecking them.
- Show live counts for pending and completed tasks.
- Play audio feedback when tasks are checked or unchecked.
- Use a dark interface with custom focus, button, checkbox, and modal styling.
- Use Bootstrap components for forms, buttons, lists, and modals.
- Keep styles, scripts, and audio assets organized in separate folders.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Bootstrap 5
- Font Awesome CDN
- HTML5 Audio API

## Project Structure

```text
application/
|-- assets/
|   `-- audios/
|       |-- complete.mp3
|       `-- uncheck.wav
|-- css/
|   `-- style.css
|-- js/
|   `-- main.js
|-- index.html
`-- README.md
```

## File Description

| File | Purpose |
| --- | --- |
| `index.html` | Main HTML file containing the app layout and Bootstrap modal markup. |
| `css/style.css` | Custom styling for the dark layout, task list, buttons, input field, checkbox, and modals. |
| `js/main.js` | JavaScript logic for adding, editing, deleting, completing, counting, and playing sounds. |
| `assets/audios/complete.mp3` | Sound played when a task is marked as complete. |
| `assets/audios/uncheck.wav` | Sound played when a completed task is moved back to the todo list. |

## How to Run

1. Download or clone this repository.
2. Open the project folder.
3. Open `index.html` in any modern web browser.

No installation or server is required.

## Usage

1. Click the input field at the bottom of the page.
2. Type a task name.
3. Press Enter to add the task.
4. Use the checkbox to mark a task as complete.
5. Click Edit to update a task.
6. Click Delete to remove a task after confirmation.
7. Uncheck a completed task to move it back to the todo list.

## Asset Paths

The app uses local audio files for task feedback. These files are stored in `assets/audios` and referenced from `js/main.js` using relative paths from `index.html`:

```js
audioplay("assets/audios/complete.mp3");
audioplay2("assets/audios/uncheck.wav");
```

The stylesheet and script are linked from `index.html` like this:

```html
<link rel="stylesheet" href="css/style.css">
<script src="js/main.js"></script>
```

## Browser Support

The application works in modern browsers that support standard DOM APIs, Bootstrap 5, and the HTML5 Audio API, including Chrome, Edge, Firefox, and Safari.

## Future Improvements

- Save tasks in local storage so they remain after refreshing the page.
- Add task due dates or priority labels.
- Improve mobile responsiveness for very small screens.
- Add filters for all, active, and completed tasks.
- Add a clear-completed action.

## Author

Created as a frontend practice project using HTML, CSS, JavaScript, and Bootstrap.
