# Employee Management System

A full-stack web application to manage employee records efficiently. The application provides an employee dashboard with CRUD operations, search, filtering, and a responsive user interface.

## 🚀 Live Demo

- **Frontend:** https://employee-management-system-ten-rho.vercel.app/
- **Backend:** https://employee-management-system-n0au.onrender.com/
- **API Health Check:** https://employee-management-system-n0au.onrender.com/api/health

## ✨ Features

- **Employee Management:** Add, view, update, and delete employee records.
- **Dashboard:** View employee statistics and records.
- **Search and Filtering:** Find employees using available filters.
- **Responsive UI:** Access the application on desktop and mobile devices.
- **REST API:** Backend API built using Node.js and Express.
- **Database Integration:** Store employee records in MongoDB Atlas.
- **Environment Variables:** Keep configuration and database credentials outside source code.

## 🛠️ Tech Stack

### Frontend
- React.js
- Vite
- CSS
- React Hooks
- Fetch API

### Backend
- Node.js
- Express.js
- Mongoose

### Database
- MongoDB Atlas

### Deployment
- Vercel (Frontend)
- Render (Backend)

## 📁 Project Structure

```text
Employee-Management-System/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   ├── package.json
│   └── .env.example
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   └── App.css
│   ├── package.json
│   └── .env.example
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

### Prerequisites

- Node.js and npm
- MongoDB Atlas account
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/shxvaamm/Employee-Management-System.git
cd Employee-Management-System
```

### 2. Set Up the Backend

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` directory using `.env.example` as a reference.

Configure the required environment variables, including your MongoDB connection string and server port.

Example:

```env
PORT=5002
MONGODB_URI=your_mongodb_connection_string
NODE_ENV=development
```

Start the backend:

```bash
npm start
```

### 3. Set Up the Frontend

Open a new terminal:

```bash
cd frontend
npm install
```

Create a `.env` file inside the `frontend` directory and configure the backend API URL:

```env
VITE_API_URL=http://localhost:5002
```

Start the frontend development server:

```bash
npm run dev
```

Open the local URL displayed in the terminal.

## 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/health` | Check backend and database status |
| GET | `/api/employees` | Retrieve employee records |
| GET | `/api/employees/:id` | Retrieve an employee by ID |
| POST | `/api/employees` | Create an employee |
| PUT | `/api/employees/:id` | Update an employee |
| DELETE | `/api/employees/:id` | Delete an employee |

## 🔐 Security

- Store database credentials in environment variables.
- Never commit `.env` files or secrets to GitHub.
- Validate incoming data on the server.
- Configure CORS for the required frontend origin.

## 🤝 Team Contribution Workflow

We follow a branch-based GitHub workflow to collaborate safely.

1. Clone the repository.
2. Create a separate branch for your assigned issue.
3. Implement the changes and test them.
4. Commit and push your branch.
5. Open a Pull Request linked to the relevant issue.
6. Wait for review and approval before merging into `main`.

**Direct pushes to `main` are not allowed.**

Example:

```bash
git checkout main
git pull origin main
git checkout -b feature/your-feature
git add .
git commit -m "feat: describe your changes"
git push -u origin feature/your-feature
```

## 📌 Future Improvements

- Authentication and role-based access control
- Improved form validation and error handling
- Additional automated tests
- Enhanced accessibility and mobile usability

## 📄 License

This project was developed as part of a college assignment. Add a license if required by your institution or project owner.
