#  Book Management Application (React + Django REST Framework)

##  Overview

The **Book Management Application** is a full-stack CRUD web app that allows users to **view, add, and manage books** with details such as title, author, price, pages, and quantity.

It’s built using a **React frontend** that communicates with a **Django REST Framework (DRF) backend** via RESTful APIs. The app demonstrates clean frontend-backend integration, API communication, and dynamic data rendering using Axios.



##  Features

*  **View All Books** – Fetches and displays all book records from the backend API.
*  **Add New Books** – Lets users add a new book by submitting a form (title, author, pages, quantity, price).
*  **Persistent Storage** – Book data is stored in the backend database via Django’s ORM.
*  **Dynamic Frontend** – Automatically updates when books are added or modified.
*  **Clean UI** – Fully responsive interface built with React Bootstrap components.

---

##  Tech Stack

### **Frontend**

*  **React.js**

  * Used for building dynamic and modular UI components.
*  **React Bootstrap**

  * Used for styling, layout, and responsive design.
*  **Axios**

  * Used for making HTTP requests to the backend API.
*  **React Router DOM**

  * Handles navigation between pages (e.g., Home and Add Book).

### **Backend**

*  **Django**

  * Handles the server-side logic and database management.
*  **Django REST Framework (DRF)**

  * Provides API endpoints for frontend communication.
*  **SQLite / PostgreSQL (depending on setup)**

  * Stores book data persistently.

---

##  Data Model

Each **Book** object has the following attributes:

| Field      | Type    | Description                        |
| ---------- | ------- | ---------------------------------- |
| `id`       | Integer | Unique identifier (auto-generated) |
| `title`    | String  | Title of the book                  |
| `author`   | String  | Author of the book                 |
| `pages`    | Integer | Number of pages in the book        |
| `quantity` | Integer | Available quantity in stock        |
| `price`    | Float   | Price of the book                  |

---

##  Folder Structure

### **Frontend (React)**

```
src/
 ├── components/
 │   └── Navbar.js          # Navigation bar
 ├── pages/
 │   ├── Home.js            # Displays book list + Add button
 │   └── AddBook.js         # Book creation form
 ├── App.js                 # Root component
 ├── index.js               # Entry point
```

### **Backend (Django)**


bookstore/
 ├── settings.py            # Django settings
 ├── urls.py                # Routes to API endpoints
 ├── models.py              # Book model
 ├── serializers.py         # Converts model to JSON
 ├── views.py               # Handles API logic
 ├── api/
 │   └── books/             # CRUD endpoints for books
```



##  API Endpoints

| Method | Endpoint           | Description             |
| ------ | ------------------ | ----------------------- |
| GET    | `/api/books/`      | Fetch all books         |
| POST   | `/api/books/`      | Create a new book       |
| GET    | `/api/books/{id}/` | Retrieve a single book  |
| PUT    | `/api/books/{id}/` | Update an existing book |
| DELETE | `/api/books/{id}/` | Delete a book           |

---

##  Skills Demonstrated

*  React fundamentals (components, props, hooks)
*  RESTful API integration
*  Axios for data fetching
*  Django REST Framework for backend APIs
*  JSON data handling between frontend and backend
*  Bootstrap UI design
*  CRUD operations implementation
*  State management using React hooks (`useState`, `useEffect`)
*  Routing using React Router



##  How It Works

1. The **frontend** loads and makes a GET request to the backend API to fetch all books.
2. The **Home** page displays all the books dynamically in a Bootstrap table.
3. Clicking **“Add New Book”** navigates to a form where users can input book details.
4. Submitting the form sends a **POST request** to the backend to create a new book record.
5. Once added, the **Home page updates** to show the new book in the list.



##  Future Improvements

*  Add “Edit” and “Delete” buttons for each book.
*  Add search and filter functionality.
*  Add pagination for long book lists.
*  Add user authentication and roles (admin, staff).
*  Add book cover image upload support.



##  Author

**Developed by:** *Abubakar Jahangir*
**Frontend:** React.js | React Bootstrap | Axios
**Backend:** Django REST Framework
**Database:** SQLite

---
