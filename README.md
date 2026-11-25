# ACTodo: To-Do App with Login

A React to-do app with login and signup pages. After logging in you land on a dashboard where you can add and delete daily activities.

## Features

- Login and Signup pages (React Router)
- Personalised dashboard header with the logged-in username
- Three static info cards on the dashboard (sample values for now)
- Add a new activity and delete existing ones

## Demo accounts

| Username | Password |
|---|---|
| `john` | `123` |
| `abc` | `123` |

New accounts created on the Signup page are kept in memory only, so they are lost on refresh. The same applies to activities.

## Tech Stack

- React 18 (Create React App)
- React Router 6
- Tailwind CSS

## Getting Started

**Prerequisites:** Node.js 18+ and npm

```bash
git clone https://github.com/BALASUBRAMANIYAN-S/project_of_TODO.git
cd project_of_TODO
npm install
npm start
```

The app opens at `http://localhost:3000`.

| Command | What it does |
|---|---|
| `npm start` | Run in development mode |
| `npm run build` | Build for production |
| `npm test` | Run tests |

## Project Structure

```
src/
├── pages/        # Login, Signup, Landing
├── components/   # Header, Card, TodoContainer, AddTodoForm, TodoList, TodoItem
├── App.js        # Routes and the in-memory user list
└── index.js
```

## Ideas for next steps

- Save users and activities in a backend or `localStorage`
- Hash passwords and add real authentication
- Hide the password field while typing (`type="password"`)
