# learnhub-frontend-# LearnHub Frontend

## 1. Project Overview

LearnHub is a web-based learning platform designed to help students access courses, interact with other learners, and track their learning progress. The frontend provides a user-friendly interface through which students and instructors can interact with the platform's features.

This project is based on the original LearnHub application and has been extended with additional learning management features.

## 2. Features

- **Course Browsing:** Allows users to explore available courses.
- **Course Learning:** Provides an interface for accessing course learning content.
- **Course Discussions:** Enables students to share ideas and participate in course-related discussions.
- **Learning Progress Tracker:** Allows students to track completed lessons and monitor their progress.
- **Course Announcements:** Provides an interface for viewing important course announcements.
- **API Integration:** Communicates with the backend to retrieve and submit application data.
- **Responsive Interface:** Designed to provide a usable experience across different screen sizes.

## 3. Technologies Used

- React
- JavaScript
- HTML5
- CSS3
- Vite
- Axios or the project's configured HTTP client
- Git and GitHub

## 4. Prerequisites

Before running the project, ensure that you have installed:

- Node.js
- npm
- Git
- The LearnHub backend application

## 5. Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/MERISHA672/learnhub-frontend.git
```

### Step 2: Enter the Project Directory

```bash
cd learnhub-frontend
```

### Step 3: Install Dependencies

```bash
npm install
```

### Step 4: Configure Environment Variables

Create a `.env` file in the frontend project root and add the following configuration:

```env
VITE_API_URL=http://localhost:5001/api
VITE_UPLOADS_URL=http://localhost:5001
```

These settings allow the frontend to communicate with the backend running on port `5001`.

Ensure the backend is configured to use the same port. Do not commit private credentials or secret environment variables to GitHub.

### Step 5: Start the Development Server

```bash
npm run dev
```

Open the local URL displayed in your terminal, commonly:

`http://localhost:5173`

## 6. Backend Integration

The frontend requires the LearnHub backend to be running for features that retrieve or save data.

Backend repository:

https://github.com/MERISHA672/learnhub-backend

Before testing the application, ensure that:

1. The backend server is running.
2. The database is configured and accessible.
3. The frontend API URL points to the correct backend address.
4. Required database tables have been created.
5. The backend permits requests from the frontend development server.

## 7. Project Structure

The project contains the following important directories and files:

```text
learnhub-frontend/
├── public/
├── src/
│   ├── components/
│   │   ├── CourseDiscussion.jsx
│   │   └── courseannouncements.jsx
│   ├── pages/
│   │   ├── public/
│   │   └── student/
│   ├── services/
│   │   ├── discussionService.js
│   │   ├── progressservice.js
│   │   └── announcementservice.js
│   ├── App.jsx
│   └── main.jsx
├── .env.example
├── .gitignore
├── package.json
└── README.md
```

*Note: The structure above highlights key files and may not list every file in the repository.*

## 8. Testing

The following areas should be tested before the final demonstration:

- Course pages load correctly.
- Course discussions reject empty messages and save valid messages.
- Learning progress remains available after refreshing the page.
- Announcements load and display correctly.
- Invalid requests display appropriate feedback.
- Backend and database connection errors are handled clearly.
- Existing login and core course workflows continue to function.

## 9. Version Control

Git was used to track project changes and GitHub to host the source code. Meaningful commits help document the development process and make changes easier to review.

## 10. Future Improvements

Possible future improvements include:

- Enhanced mobile responsiveness.
- Improved accessibility.
- More detailed student progress reports.
- Notifications for new announcements.
- Additional automated tests.

## 11. Acknowledgement

This project builds upon the original LearnHub application provided for the Web and Mobile Application Development assignment. The original project is credited to its respective authors. Additional features and modifications are documented as part of the coursework.

AI assistance was used during development for guidance, troubleshooting, and documentation. The submitted code and functionality should be reviewed and verified by the student.

## 12. Author

**Name:** Melissa [Insert Full Name]  
**Course:** Bachelor of Science in Information Technology (BSIT)  
**Institution:** Uganda Christian University  
**Project:** Web and Mobile Application Development Assignment

---

**Repository:** https://github.com/MERISHA672/learnhub-frontend
