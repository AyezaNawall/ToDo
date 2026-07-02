# Todo Application

A clean, browser-based todo application built with HTML, CSS, JavaScript, and Bootstrap. This project lets users create, edit, delete, and complete tasks through a simple dark-themed interface with interactive controls and audio feedback.

## Overview

This repository contains a lightweight frontend todo app that runs directly in the browser. It does not require a backend, database, or build setup. The application focuses on essential task management actions while keeping the interface minimal, responsive, and easy to use.

Users can add tasks, track how many tasks are still pending, move completed tasks into a separate completed section, edit existing task text, and confirm deletion before removing a task.

## Features

- Add new tasks by typing into the input field and pressing Enter.
- Edit existing tasks using a Bootstrap modal.
- Delete tasks with a confirmation modal to prevent accidental removal.
- Mark tasks as complete using a checkbox.
- Move completed tasks into a dedicated completed section.
- Restore completed tasks back to the todo list by unchecking them.
- Display live task counts for pending and completed tasks.
- Play audio feedback when tasks are checked or unchecked.
- Use a dark user interface with custom focus and button styling.
- Use Bootstrap components for buttons, lists, forms, and modals.
- Keep audio files organized inside the `audios` folder.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Bootstrap 5
- Font Awesome CDN
- Browser Audio API

## Project Structure

```text
application/
├── audios/
│   ├── myaudio.mp3
│   └── no2.wav
├── readme.md
├── todo.css
├── todo.html
└── todo.js
```

## File Description

| File                 | Purpose                                                                                    |
| -------------------- | ------------------------------------------------------------------------------------------ |
| `todo.html`          | Main HTML structure for the todo interface and Bootstrap modals.                           |
| `todo.css`           | Custom styling for the dark layout, task items, buttons, input field, and modals.          |
| `todo.js`            | Application logic for adding, editing, deleting, completing, counting, and playing sounds. |
| `audios/myaudio.mp3` | Sound played when a task is marked as complete.                                            |
| `audios/no2.wav`     | Sound played when a task is moved back to the todo list.                                   |

## How to Run

1. Download or clone this repository.
2. Open the project folder.
3. Open `todo.html` in any modern web browser.

No installation, server, or package manager is required.

## Usage

1. Click the input field at the bottom of the page.
2. Type a task name.
3. Press Enter to add the task.
4. Use the checkbox to mark a task as complete.
5. Click Edit to update a task.
6. Click Delete to remove a task after confirmation.
7. Uncheck a completed task to move it back to the todo list.

## Audio Assets

The app uses local audio files for task status feedback. These files are stored in the `audios` directory and are referenced from `todo.js` using relative paths:

Keep the audio files in this folder unless you also update the paths in `todo.js`.

## Browser Support

The application works in modern browsers that support standard DOM APIs, Bootstrap 5, and the HTML5 Audio API, including:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

## Future Improvements

- Save tasks in local storage so they remain after refreshing the page.
- Add task due dates or priority labels.
- Improve mobile responsiveness for very small screens.
- Add filters for all, active, and completed tasks.
- Add a clear-completed action.

## Author

Created as a frontend practice project using HTML, CSS, JavaScript, and Bootstrap.
