# Book Management System

A modern responsive React Book Management System built with React, HTML, CSS, JavaScript, Bootstrap, Axios, React Router DOM, and JSON Server.

## Features

- Responsive Bootstrap book cards on the home page
- Book details page with React Router
- Search by title or author
- Filter by genre
- Admin dashboard with total book count and genre statistics
- Four book type divisions: Religious Books, Historical Books, Fiction/Novels, and Educational Books
- Add, edit, and delete book records
- JSON Server backend at `http://localhost:5000/books`
- Loading spinner, error messages, empty states, delete confirmation, and success toasts

## Project Structure

```text
src/
 ├── components/
 │     ├── Navbar.js
 │     ├── Footer.js
 │     ├── BookCard.js
 │     ├── SearchBar.js
 │     ├── GenreFilter.js
 │     ├── Loader.js
 │     └── BookForm.js
 ├── pages/
 │     ├── Home.js
 │     ├── BookDetails.js
 │     ├── Dashboard.js
 │     ├── AddBook.js
 │     └── EditBook.js
 ├── services/
 │     └── api.js
 ├── App.js
 └── index.js
```

This Vite project uses `src/App.jsx` and `src/main.jsx`, which are the Vite equivalents of `App.js` and `index.js`.

## Setup

Install dependencies:

```bash
npm install
```

Start JSON Server:

```bash
npm run server
```

Start the React app in a second terminal:

```bash
npm run dev
```

Open the local URL shown by Vite, usually:

```text
http://localhost:5173
```

## API Endpoints

JSON Server reads from `db.json` and exposes:

- `GET /books`
- `POST /books`
- `PUT /books/:id`
- `DELETE /books/:id`

Base URL used by Axios:

```text
http://localhost:5000/books
```

## Routes

- `/`
- `/book/:id`
- `/admin`
- `/add-book`
- `/edit-book/:id`
