
Rust Python Compiler (Web-based)

A web-based online Python compiler built using Rust with:

Leptos (Frontend)

Axum (Backend)

Monaco Editor (Code Editor)

Docker (Python Execution)


Features

✅ Role-based Authentication
✅ Inbuilt Code Editor (VS Code-style)
✅ Run Button to Execute Python Code
✅ Console to Display Program Output
✅ Secure Execution in Docker


---

Project Structure

rust_python_compiler/
│── backend/   (Rust API - Handles user authentication & execution)
│── frontend/  (Rust + Leptos - UI with Monaco Editor)
│── executor/  (Docker-based Python execution)


---

Installation & Setup

1. Prerequisites

Rust (cargo)

Node.js (for trunk & frontend)

Docker (for Python execution)

PostgreSQL (for user authentication)


2. Clone the Repository

git clone https://github.com/your-repo/rust_python_compiler.git
cd rust_python_compiler

3. Backend Setup

cd backend
cargo build --release
cargo run

4. Frontend Setup

cd frontend
trunk serve

5. Run Docker for Python Execution

docker run --rm -it python:3.10 python


---

How It Works

1. User Logs In

Uses PostgreSQL for authentication.



2. User Writes Python Code in the Editor

Monaco Editor provides an interactive coding experience.



3. User Clicks "Run"

The backend sends the code to a Docker container for execution.



4. Output is Displayed in the Console

The result is fetched from the container and displayed.





---

Technologies Used

Rust (Axum, Leptos) → Backend & Frontend

Docker → Secure Python Execution

Monaco Editor → Code Editor

PostgreSQL → User Authentication



---

Future Enhancements

Improve role-based access (Admin/User)

Add syntax error highlighting

Store execution history 
