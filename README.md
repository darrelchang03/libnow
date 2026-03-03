# libnow A full-stack web application built to manage an online library — enabling users to browse, borrow and return books in a streamlined and user-friendly interface.

## Project Overview

**libnow** is designed as a modern digital library system built with JavaScript, Node.js, and Express, with EJS templating and MongoDB (or your choice of database) for data persistence. Through this project I learned end-to-end web app skills: front-end views, back-end logic, routing, and data modelling.

### Key features
- Book catalog view: list all available books, view details, cover images.  
- CRUD operations for books (Add / Edit / Delete) via intuitive UI.  
- Data modelling with Mongoose (or equivalent) for Books, Users and BorrowRecords.  
- Express routing handling API endpoints and server-side views.  
- EJS templated views in `views/` folder for dynamic rendering.  
- Public assets (CSS, JS, covers) under `public/` directory.  
- Modular project structure: `models/`, `routes/`, `views/`, `public/`, etc.  
- Ready for hosting / deployment (e.g., Heroku, Render, or Vercel-Serverless).  

---

## Stack

| Runtime        | Node.js                                     |
| Web Framework  | Express.js                                  |
| Templating     | EJS                                         |
| Database       | MongoDB (via Mongoose)                      |
| Front-end      | HTML5, CSS3, client-side JavaScript         |
| Project Structure | MVC-inspired: models, routes, views, public assets |
| Version Control| Git + GitHub                                |

## Project Structure
e-library/
│ server.js ← entry point
│ package.json ← npm dependencies & scripts
│
├── models/ ← database models (Book, User, BorrowRecord, …)
├── routes/ ← Express route handlers
├── views/ ← EJS templates for rendering UI
├── public/ ← static assets: stylesheets, client JS, book covers
└── … additional files/folders …

---

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/darrelchang03/e-library.git
   cd e-library
  
2. Install dependencies:
   ```bash
    npm install

3. Create a .env file (if using environment variables) with entries such as:
   ```env
    MONGODB_URI=your_mongodb_connection_string
    PORT=3000

4. Start the development server:
    ```bash
    npm start

5. Open your browser and navigate to http://localhost:3000 (or whichever port you changed it to).

## What I Learned / Challenges

Designed and implemented a full REST-style back-end with Express & MongoDB.

Built server-rendered views with EJS and integrated front-end & back-end logic.

Managed asynchronous code (e.g., database operations) and error handling.

Established a clean project architecture (models/routes/views) for scalability and maintainability.

Faced and addressed common challenges such as: routing conflicts, database indexing, cover image uploads/serving (Multer).

---

## Future Improvements

Add user authentication & authorization (e.g., using Passport.js, bcrypt) so only logged-in users can borrow/return books.

Add book reservation/wait-list functionality.

Introduce filters/sorting: by genre, author, availability, publication date.

Integrate with a third-party storage (AWS S3, Cloudinary).

Improve UI/UX: responsive design, better styling/themes, client-side dynamic updates (AJAX).

