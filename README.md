# ChatttingWeb: Full-Stack Learning & Chat Management
ChatttingWeb is a real-time communication platform designed for academic environments. It combines instant messaging with classroom features like assignment submissions, folder-based material management, and user authentication.

# Key Features
Real-Time Chat: WebSocket-driven messaging with support for multiple chat rooms and member management (invite/kick).
Classroom Materials: Organize educational content using a nested folder system and file uploads.
Assignment System: Teachers can post assignments with due dates, and students can submit files directly through the app.
Secure Authentication: JWT-based authentication with bcrypt password hashing.
Dynamic UI: A React-based frontend featuring emoji pickers, file previews, and a responsive layout.

# Technical Stack
Backend (FastAPI)
Framework: FastAPI (Python)
ORM: SQLAlchemy with PostgreSQL
Real-time: WebSockets
Security: JWT Tokens & Passlib (Bcrypt)
Frontend (React)
Framework: React 18+ (Vite)
Routing: React Router DOM
Communication: Socket.io-client & Fetch API
Styling: Custom CSS with interactive animations

# Repository Structure
Backend:
main.py: The application entry point and CORS configuration.
models.py: SQLAlchemy database schemas (Users, Rooms, Messages, Folders, Assignments).
auth.py: Logic for token generation and password verification.
chat.py: WebSocket endpoints and room logic.
meterial.py: Material uploads and folder management.
assignment.py: Teacher posts and student submissions.
users.py: Registration and login handlers.

Frontend:
main.jsx: React DOM entry point.
App.jsx: Route definitions (/login, /home, /register).
Webpage.jsx: The core UI logic, including chat windows and file explorers.
App.css: Global styles and UI animations.
