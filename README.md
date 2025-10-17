# Kaiburr Task 3 - Task Manager Web UI

## 📋 Overview

This is the frontend UI for the Kaiburr Task Manager application, built using **React 19**, **TypeScript**, and **Ant Design**. It provides a modern, responsive interface to interact with the backend API from Task 1/Task 2, enabling users to create, view, and delete task records.

## ✨ Features

- ✅ **Create Tasks** - Add new tasks with ID, name, owner, and command
- ✅ **View Tasks** - Display all existing tasks in a clean table format
- ✅ **Delete Tasks** - Remove tasks with a single click
- ✅ **Responsive Design** - Built with Ant Design for a professional look
- ✅ **Real-time Updates** - Instant feedback on all operations
- ✅ **Error Handling** - User-friendly error messages and notifications

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| **Framework** | React 19 |
| **Language** | TypeScript |
| **UI Library** | Ant Design |
| **HTTP Client** | Axios |
| **Backend API** | Spring Boot (Task 2, NodePort 30080) |

## 📁 Project Structure

```
TASK-MANAGER-UI/
├── public/
├── Screenshots/
└── src/
    ├── App.tsx
    ├── index.css
    └── index.tsx
```

## 🚀 Setup and Run

### Prerequisites

- **Node.js** 18 or higher
- **npm** or **yarn**
- Backend API running (from Task 2) at `http://localhost:30080`

### Installation

#### 1. Clone the repository

```bash
git clone https://github.com/karthik74066/task-manager-ui.git
cd task-manager-ui
```

#### 2. Install dependencies

```bash
npm install
```

#### 3. Start the application

```bash
npm start
```

The development server will run at:
```
http://localhost:3000
```

### Build for Production

```bash
npm run build
```

This creates an optimized production build in the `build/` folder.

## 🔌 Backend Integration

The UI connects to the Spring Boot backend at:
```
http://localhost:30080/api/tasks
```

Ensure the backend service is running before starting the UI.

## 🖼️ Screenshots

Screenshots of the application are available in the `Screenshots/` directory.

## 📋 Available Scripts

| Command | Description |
|---------|-------------|
| `npm start` | Runs the app in development mode |
| `npm test` | Launches the test runner |
| `npm run build` | Builds the app for production |
| `npm run eject` | Ejects from Create React App (one-way operation) |

## 🔧 Configuration

To change the backend API URL, update the axios base URL in `App.tsx`:

```typescript
const API_BASE_URL = 'http://localhost:30080/api/tasks';
```

## 🧪 Testing

### Manual Testing Steps

1. **Create a Task**
   - Fill in the form with task details
   - Click "Create Task"
   - Verify the task appears in the table

2. **View Tasks**
   - Check that all tasks are displayed correctly
   - Verify all fields are visible

3. **Delete a Task**
   - Click the "Delete" button for any task
   - Confirm the task is removed from the list

## 🐛 Troubleshooting

### Backend Connection Issues

If you see connection errors:
- Verify the backend is running at `http://localhost:30080`
- Check that CORS is enabled in the backend
- Ensure MongoDB is running and connected

### Port Already in Use

If port 3000 is busy:
```bash
# Find and kill the process
npx kill-port 3000

# Or run on a different port
PORT=3001 npm start
```

## 👨‍💻 Author

**Name:** Karthik S  
**Project:** Kaiburr Assessment - Task 3  
**Date:** October 2025  
**GitHub:** [@karthik74066](https://github.com/karthik74066)

## 📄 License

This project is part of the Kaiburr Assessment.

## 🤝 Contributing

This is an assessment project and is not open for contributions.

---

For questions or issues, please contact the author.