📝 MERN Todo App
A full-stack Todo application built with the MERN stack (MongoDB, Express.js, React, Node.js). This project is perfect for beginners learning full-stack development.

🌟 Features
✅ Add new todos

✅ View all todos

✅ Delete todos

✅ Real-time updates

✅ MongoDB cloud database

✅ RESTful API

✅ Responsive design

🛠️ Tech Stack
Frontend:

React.js

Axios for API calls

CSS for styling

Backend:

Node.js

Express.js

MongoDB (Atlas - Cloud)

Mongoose ODM

CORS for cross-origin requests

🚀 Quick Start
Prerequisites
Node.js (v14 or higher)

npm or yarn

MongoDB Atlas account (free)

Installation
Clone the repository

bash
git clone https://github.com/snigdhadwiv/mern-todo-app.git
cd mern-todo-app
Set up Backend

bash
cd backend
npm install
Configure Environment Variables
Create a .env file in the backend folder:

env
MONGODB_URI=mongodb+srv://your_username:your_password@cluster0.mongodb.net/todoapp?retryWrites=true&w=majority
PORT=5000
Set up Frontend

bash
cd ../frontend
npm install
Running the Application
Start Backend Server:

bash
cd backend
npm run dev
Server runs at: http://localhost:5000

Start Frontend:

bash
cd frontend
npm start
App opens at: http://localhost:3000

📁 Project Structure
text
mern-todo-app/
├── backend/
│   ├── server.js          # Express server & API routes
│   ├── package.json       # Backend dependencies
│   └── .env              # Environment variables
├── frontend/
│   ├── src/
│   │   ├── App.js        # Main React component
│   │   ├── App.css       # Styles
│   │   └── index.js      # React entry point
│   └── package.json      # Frontend dependencies
└── README.md
🔧 API Endpoints
Method	Endpoint	Description
GET	/api/todos	Get all todos
POST	/api/todos	Create new todo
DELETE	/api/todos/:id	Delete a todo
🎯 How It Works
Frontend (React): User interacts with the UI

API Calls: Frontend sends HTTP requests to backend

Backend (Express): Processes requests, talks to database

Database (MongoDB): Stores todos persistently

Response: Data flows back to frontend for display

📦 Database Schema
javascript
{
  text: String,        // Todo text (required)
  completed: Boolean,  // Completion status (default: false)
  createdAt: Date,     // Auto-generated timestamp
  updatedAt: Date      // Auto-generated timestamp
}
🚦 Running Tests
bash
# Backend tests (if implemented)
cd backend
npm test

# Frontend tests
cd frontend
npm test
🔐 Security Notes
Never commit .env files to version control

Use environment variables for sensitive data

MongoDB Atlas provides free cloud database

CORS is configured for local development

📚 Learning Points
This project covers:

Setting up MongoDB Atlas (cloud database)

Creating Express.js REST API

Building React frontend with Hooks

Connecting frontend to backend

Handling CRUD operations

Using environment variables

Git and GitHub workflow

🔄 Deployment
Frontend (Vercel)
Push code to GitHub

Connect repo to Vercel

Set root directory to frontend

Add environment variable: REACT_APP_API_URL

Backend (Render/Railway)
Create web service

Set start command: node server.js

Add environment variables

Update MongoDB IP whitelist

🤝 Contributing
Fork the repository

Create a feature branch

Commit your changes

Push to the branch

Open a Pull Request

📄 License
This project is open source and available under the MIT License.

🙏 Acknowledgements
MongoDB Atlas for free cloud database

Create React App for boilerplate

Express.js team

React team

📞 Support
For support, open an issue in the GitHub repository or contact the maintainer.

Built with ❤️ using the MERN stack
GitHub: https://github.com/snigdhadwiv/mern-todo-app

✨ Future Enhancements
User authentication

Edit todo functionality

Mark as complete toggle

Categories/Tags

Due dates

Search/filter todos

Dark mode

COMPLETE TIMELINE - WHAT WE DID
PHASE 1: MONGODB SETUP
Went to mongodb.com → Signed up for free account
Created "Cluster0" → Free tier MongoDB cloud database
Added IP address 106.222.212.63 → Allowed local connection
Created database user: sigusac_db_user with password
Got connection string: mongodb+srv://sigusac_db_user:5lpOySWrhrHDIAxX@cluster0.2ljm0qi.mongodb.net/?appName=Cluster0
Modified string: Added /todoapp for database name
PHASE 2: INITIAL VS CODE SETUP
Opened VS Code → New window
Terminal (Ctrl + ) →mkdir merntodo` → Failed attempt
Started fresh → mkdir mern-project
PHASE 3: BACKEND CREATION
cd mern-project → Enter project
mkdir backend → Create backend folder
cd backend → Enter backend
npm init -y → Initialize Node.js project
npm install express mongoose cors dotenv nodemon → Install all packages
Created .env file → Added MongoDB URI + PORT
Created server.js → Backend code
Updated package.json → Added start/dev scripts
node server.js → Test → ✅ SUCCESS!
PHASE 4: FRONTEND (NEXT)
Will create React frontend that connects to this backend

WHAT EACH COMMAND DID
MongoDB Setup:
mongodb+srv://... → Cloud database address
/todoapp → Database name inside MongoDB
?retryWrites=true&w=majority → Connection settings
Terminal Commands:
mkdir → Make directory (folder)
cd → Change directory (move into folder)
npm init -y → Create package.json with default answers
npm install → Download packages from internet
node server.js → Run JavaScript file
File Structure Created:
text
mern-project/
└── backend/
    ├── node_modules/     # All installed packages
    ├── .env             # Secrets (MongoDB password)
    ├── server.js        # Main backend code
    ├── package.json     # Project info & commands
    └── package-lock.json # Exact package versions

NEXT STEPS
Now we'll create the React frontend that:
Runs on localhost:3000
Sends requests to localhost:5000
Displays todos from MongoDB
Can add/delete todos
COMPLETE PROJECT TIMELINE
PHASE 1: MONGODB SETUP
Went to mongodb.com → Signed up for free account
Created "Cluster0" → Free tier MongoDB cloud database
Added IP address 106.222.212.63 → Allowed local connection
Created database user: sigusac_db_user with password
Got connection string: mongodb+srv://sigusac_db_user:5lpOySWrhrHDIAxX@cluster0.2ljm0qi.mongodb.net/?appName=Cluster0
Modified string: Added /todoapp for database name
PHASE 2: INITIAL VS CODE SETUP
Opened VS Code → New window
Terminal (Ctrl + ) →mkdir merntodo` → Failed attempt
Started fresh → mkdir mern-project
PHASE 3: BACKEND CREATION
cd mern-project → Enter project
mkdir backend → Create backend folder
cd backend → Enter backend
npm init -y → Initialize Node.js project
npm install express mongoose cors dotenv nodemon → Install all packages
Created .env file → Added MongoDB URI + PORT
Created server.js → Backend code
Updated package.json → Added start/dev scripts
node server.js → Test → ✅ SUCCESS!
PHASE 4: FRONTEND CREATION
cd .. → Back to project root
npx create-react-app frontend → Create React app
cd frontend → Enter frontend
npm install axios → Install HTTP client
Updated App.js → Added todo functionality
Updated App.css → Added styling
PHASE 5: RUNNING THE APP
Terminal 1: cd backend → npm run dev → Backend: localhost:5000
Terminal 2: cd frontend → npm start → Frontend: localhost:3000
Tested: Add/Delete todos → Works with MongoDB!
PHASE 6: GIT & GITHUB
cd .. → Back to project root
git init → Initialize git
Created .gitignore → Excluded node_modules, .env
git add . → Add files
git commit -m "Initial commit" → First commit
Created GitHub repo: mern-todo-app
git remote add origin https://github.com/snigdhadwiv/mern-todo-app.git
git branch -M main
git push -u origin main → ✅ Pushed to GitHub!

SERVER STARTING COMMANDS (KEEP HANDY)
TO START THE APP ANYTIME:
Method 1: Two Terminal Windows
Terminal 1 (Backend):
bash
cd backend
npm run dev
Output: 🚀 Server running on http://localhost:5000
Terminal 2 (Frontend):
bash
cd frontend
npm start
Output: Opens http://localhost:3000 in browser
Method 2: VS Code Split Terminal
Open VS Code to your project
Ctrl + Shift + 5 (split terminal)
Left pane: cd backend && npm run dev
Right pane: cd frontend && npm start
Method 3: Quick Start Script
Create start.bat (Windows) or start.sh (Mac/Linux):
start.bat:
batch
@echo off
start cmd /k "cd backend && npm run dev"
timeout /t 2
start cmd /k "cd frontend && npm start"
start.sh:
bash
#!/bin/bash
cd backend && npm run dev &
sleep 2
cd frontend && npm start

TROUBLESHOOTING COMMANDS
If Backend Won't Start:
bash
# Check if port 5000 is in use
netstat -ano | findstr :5000

# Kill process on port 5000
taskkill /PID [PID_NUMBER] /F

# Reinstall backend dependencies
cd backend
rmdir /s node_modules
npm install
npm run dev
If Frontend Won't Start:
bash
# Clear cache
cd frontend
npm cache clean --force

# Reinstall
rmdir /s node_modules
npm install
npm start
If MongoDB Connection Fails:
Check .env file has correct connection string
Check MongoDB Atlas: Network Access → Your IP is whitelisted
Test connection: node backend/server.js

PROJECT STRUCTURE
text
mern-project/
├── backend/
│   ├── .env                    # MongoDB credentials (KEEP SECRET!)
│   ├── server.js              # Backend API code
│   ├── package.json           # Backend dependencies
│   └── node_modules/          # Backend packages
├── frontend/
│   ├── src/
│   │   ├── App.js            # Main React component
│   │   ├── App.css           # Styles
│   │   └── index.js          # React entry point
│   ├── package.json          # Frontend dependencies
│   └── node_modules/         # Frontend packages
└── .gitignore                # Git ignore rules

QUICK REFERENCE
URLs:
Frontend: http://localhost:3000
Backend API: http://localhost:5000
API Endpoints:
GET /api/todos → Get all todos
POST /api/todos → Add new todo
DELETE /api/todos/:id → Delete todo
Git Commands:
bash
# Update code
git add .
git commit -m "Your message"
git push

# Pull updates
git pull

# Check status
git status
Installation (Fresh Clone):
bash
# Clone from GitHub
git clone https://github.com/snigdhadwiv/mern-todo-app.git
cd mern-todo-app

# Install backend
cd backend
npm install
# Create .env file with your MongoDB URI
# Add: MONGODB_URI=your_connection_string

# Install frontend
cd ../frontend
npm install

# Start both servers (in two terminals)

YOUR PROJECT IS NOW:
✅ Complete MERN Stack Application
✅ GitHub Repository: https://github.com/snigdhadwiv/mern-todo-app
✅ Working locally (localhost:3000 & 5000)
✅ Cloud database (MongoDB Atlas)
✅ Ready to expand (add features, deploy, etc.)
To run anytime: Just open VS Code, split terminal, run those two commands! 🚀

