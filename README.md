# Planify

Planify is a task management web application designed to help users efficiently organize, track, and complete their tasks. With its user-friendly interface and productivity-focused features, Planify ensures users stay on top of their responsibilities while prioritizing effectively.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Features
1. **Task Creation & Tracking**  
   - Users can easily create, view, and manage tasks.
   - Tasks are categorized as completed, pending, or overdue based on deadlines and progress.

2. **Priority Levels**  
   - Tasks can be classified by priority: Low, Medium, High.

3. **User Dashboard**  
   - Provides an overview of tasks, including total tasks, tasks in progress, and completed tasks.
   - Visualizes task completion stats and activity trends to keep users motivated.

4. **Responsive Design**  
   - Seamless experience across devices (desktop, tablet, mobile).

## Technologies Used
- **Frontend**: React.js, Next.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (Mongoose)
- **Authentication**: JSON Web Tokens (JWT)
- **Hosting**: Vercel (Frontend), Render/Heroku (Backend)

## Installation
Follow these steps to run Planify locally:

### 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/Planify.git
cd Planify
```

### 2. Setup the Backend
Navigate to the `backend` directory and install dependencies:
```bash
cd backend
npm install
```

Create a `.env` file in the `backend` folder with the following variables:
```
MONGO_URI=<your-mongodb-connection-string>
JWT_SECRET=<your-secret-key>
CLIENT_URL=http://localhost:3000
PORT=8000
```

Start the backend server:
```bash
nodemon server.js
```

### 3. Setup the Frontend
Navigate to the `client` directory and install dependencies:
```bash
cd ../client
npm install
```

Start the frontend development server:
```bash
npm run dev
```

Access the application at `http://localhost:3000`.

## Usage
1. **Login/Register**
   - Create an account or log in to access your personalized dashboard.

2. **Add Tasks**
   - Create tasks, assign priorities, and set deadlines.

3. **Track Progress**
   - Monitor your task status on the dashboard and adjust as needed.

4. **Analyze Productivity**
   - Use completion stats and visual trends to improve your workflow.

## API Endpoints

### Authentication
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/login` | POST | Login a user |
| `/api/auth/register` | POST | Register a new user |

### Tasks
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/tasks` | GET | Fetch all tasks |
| `/api/tasks` | POST | Create a new task |
| `/api/tasks/:id` | PATCH | Update an existing task |
| `/api/tasks/:id` | DELETE | Delete a specific task |

## Contributing
We welcome contributions from the community! If you'd like to contribute:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
Planify was developed by a collaborative team:
- Daffa Ramzy Saputra
- James Michael Siswanto
- M. Faisal Syahwaludin
- M. Zakiy Mubarok
- Nathanael Setiawan
- Pangeran Maharesi Dunia
- Pradipa Wibi Herdani

Special thanks to everyone who contributed their time, effort, and creativity to this project.
