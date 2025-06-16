# Job Hunter

Job Hunter is a full-stack web application for searching, organizing, and managing job applications in one place.

## 🚀 Tech Stack

### 🔧 Frontend

- *React.js*: Component-based UI
- *Redux*: State management
- *React Router*: SPA routing
- *Axios*: HTTP requests
- *Bootstrap / Material-UI*: Responsive, styled components

### 🛠 Backend

- *Node.js*: Backend runtime
- *Express.js*: RESTful API framework
- *MongoDB*: NoSQL database
- *Mongoose*: ODM for MongoDB
- *JWT*: Authentication

## 🔍 How It Works

1. *User Registration & Authentication*
    - Sign up/login with email & password
    - JWT-based authentication
    - Protected routes for dashboard & jobs

2. *Job Application Management*
    - Add, edit, delete job applications
    - Fields: company, position, status, notes, deadlines
    - View jobs in table/card layout

3. *Dashboard Overview*
    - Application summary
    - Visual analytics (charts/graphs)
    - Filter by company, status, date
    - Quick access to interviews

4. *Frontend-Backend Communication*
    - RESTful API endpoints:
      - /api/auth/* (auth)
      - /api/jobs/* (jobs)
    - Axios for requests
    - UI notifications for errors/responses

5. *Data Persistence*
    - MongoDB for storage
    - Mongoose schemas for validation
    - User-specific data via JWT

## 🛠 Getting Started

1. *Install Dependencies*
    - *Backend*
      bash
      cd backend
      npm install
      
    - *Frontend*
      bash
      cd ../frontend
      npm install
      

2. *Set Environment Variables*
    - In backend/.env:
      
      MONGO_URI=your_mongodb_connection_string
      JWT_SECRET=your_jwt_secret_key
      PORT=5000
      

3. *Run the Application*
    - *Backend*
      bash
      npm start
      
    - *Frontend* (in new terminal)
      bash
      cd frontend
      npm start
      
    - Frontend: [http://localhost:3000](http://localhost:3000)  
      Backend: [http://localhost:5000](http://localhost:5000)

## 🌟 Key Features

- 🔐 *Authentication* – JWT-based login/registration
- 🗃 *Job Tracker* – Add, update, manage applications
- 📊 *Dashboard Analytics* – Job hunt stats
- 🔍 *Search & Filter* – Sort/find applications
- 🌐 *RESTful API* – Clean backend endpoints
- 🖥 *Responsive UI* – Desktop, tablet, mobile

## 📁 Folder Structure


job-hunter/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── server.js
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── redux/
│   │   ├── App.js
│   │   └── index.js


## 🚧 Future Enhancements

- 📅 Calendar view for interviews
- 🔔 Email reminders/push notifications
- 📥 Resume uploader/job-saving
- 🌍 Job board scraping & auto-fill

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Fork the repo and submit a pull request.

## 📄 License

MIT License

---

# 🖥 VS Code Workspace Setup

## 1. Open the Project

bash
code job-hunter

Or use *File > Open Folder...* in VS Code.

## 2. Recommended Extensions

- ESLint
- Prettier
- MongoDB for VS Code
- REST Client
- GitLens

## 3. Workspace Settings Example

Create .vscode/settings.json:

json
{
     "editor.formatOnSave": true,
     "files.exclude": {
          "**/node_modules": true,
          "**/.env": true
     },
     "eslint.enable": true,
     "prettier.requireConfig": true
}


## 4. Debugging

- Backend: Add .vscode/launch.json for Node.js
- Frontend: Use Debugger for Chrome or browser debugging

## 5. Scripts

Use the terminal (`Ctrl + ``):

- npm start (backend)
- npm start (frontend, in frontend/)

## 6. Multi-root Workspace (Optional)

- *File > Add Folder to Workspace...*
- Add backend and frontend
- Save as job-hunter.code-workspace

---

VS Code streamlines development with linting, formatting, and integrated terminal support.
