
# **Bible App**
**An engaging, dynamic, and interactive web app for Iglesia Bautista Pan de Vida.** This app includes schedules, predications, games, a children's church section, and community interaction features.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technology Stack](#technology-stack)
4. [Getting Started](#getting-started)
5. [Directory Structure](#directory-structure)
6. [Contributing](#contributing)
7. [License](#license)

---

## **Project Overview**
The Bible App is designed to bring the community closer through:
- Dynamic church schedules.
- Predication videos and Bible study guides.
- Bible-based games for adults and children.
- A dedicated area for children's church content.
- Community features like prayer requests and donation tracking.

---

## **Features**
- **Dynamic Content**: Manage schedules, Bible guides, and predications via an admin panel.
- **Interactive Games**:
  - Trivia quiz.
  - Fill-in-the-blank Bible verses.
  - Memory and coloring games for children.
- **Children's Section**: Bible stories, games, and sing-along hymns.
- **Community Engagement**: Prayer requests and donation system.
- **Responsive Design**: Optimized for both desktop and mobile devices.

---

## **Technology Stack**
### **Frontend**:
- React
- TailwindCSS / Material-UI for styling
- Axios for API communication

### **Backend**:
- Node.js with Express.js
- Database: PostgreSQL (via Sequelize) or MongoDB (via Mongoose)

### **Testing**:
- Jest
- React Testing Library

### **Deployment**:
- Docker
- Netlify (Frontend) + Heroku (Backend)

---

## **Getting Started**

### **Prerequisites**
- Node.js and npm installed on your machine.
- Docker (optional for deployment).

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/bible-app.git
   cd bible-app
   ```

2. Set up the backend:
   ```bash
   cd backend
   npm install
   cp .env.example .env  # Configure database credentials
   npm run dev           # Start backend server
   ```

3. Set up the frontend:
   ```bash
   cd frontend
   npm install
   npm start             # Start React development server
   ```

4. Open the app in your browser at `http://localhost:3000`.

---

## **Directory Structure**
Here’s an overview of the main directories:

```plaintext
bible-app/
├── backend/                                # Backend API and server logic
│   ├── controllers/                        # Business logic for different features
│   │   ├── triviaController.js             # Trivia game logic
│   │   ├── scheduleController.js           # Church schedule logic
│   │   ├── storyController.js              # Children's Bible stories logic
│   │   ├── userController.js               # User authentication and progress tracking
│   ├── models/                             # Database models and schemas
│   │   ├── Trivia.js                       # Trivia questions schema
│   │   ├── Schedule.js                     # Church schedule schema
│   │   ├── BibleStory.js                   # Bible stories schema
│   │   ├── User.js                         # User account schema
│   ├── routes/                             # API routes
│   │   ├── triviaRoutes.js                 # Endpoints for trivia game
│   │   ├── scheduleRoutes.js               # Endpoints for schedule
│   │   ├── storyRoutes.js                  # Endpoints for Bible stories
│   │   ├── userRoutes.js                   # Endpoints for user authentication
│   ├── db/                                 # Database configuration and migrations
│   │   ├── config.js                       # Database connection settings
│   │   ├── migrations/                     # Database migration scripts
│   │   ├── seeders/                        # Seed data for initial setup
│   ├── utils/                              # Helper utilities
│   │   ├── validators.js                   # Input validation utilities
│   │   ├── errorHandler.js                 # Centralized error handling
│   ├── tests/                              # Backend tests
│   │   ├── testSchedule.js                 # Tests for schedule feature
│   │   ├── testTrivia.js                   # Tests for trivia game
│   ├── server.js                           # Entry point for backend
│   ├── package.json                        # Backend dependencies
│   ├── .env.example                        # Sample environment variables for backend
├── frontend/                               # Frontend React application
│   ├── public/                             # Static files served by React
│   │   ├── index.html                      # Root HTML file for React app
│   │   ├── images/                         # Static images for UI
│   │   │   ├── ark.png
│   │   │   ├── cross.png
│   │   │   ├── church_logo.png
│   │   └── styles/                         # Global CSS files
│   │       ├── main.css                    # Main CSS file
│   │       ├── children.css                # Styles for children's section
│   ├── src/
│   │   ├── components/                     # Reusable UI components
│   │   │   ├── Header.js                   # Header navigation bar
│   │   │   ├── Footer.js                   # Footer with contact info
│   │   │   ├── Schedule.js                 # Displays church schedules
│   │   │   ├── VideoSection.js             # YouTube video embeds
│   │   │   ├── Guide.js                    # Bible study guide display
│   │   │   ├── TriviaQuiz.js               # Trivia quiz game component
│   │   │   ├── FillInTheBlank.js           # Fill-in-the-blank game
│   │   │   ├── MemoryGame.js               # Memory game for children
│   │   │   ├── ColoringBook.js             # Coloring book for children
│   │   │   ├── ChildrenSection.js          # Contains children's activities
│   │   │   ├── AdultGames.js               # Bible games for adults
│   │   ├── pages/                          # Pages for routing
│   │   │   ├── HomePage.js                 # Main page with church info
│   │   │   ├── GamesPage.js                # Games hub for adults and children
│   │   │   ├── StoriesPage.js              # Bible stories listing
│   │   │   ├── ContactPage.js              # Contact information
│   │   ├── utils/                          # Utility functions for frontend
│   │   │   ├── api.js                      # Helper functions for API calls
│   │   ├── App.js                          # Main React App component
│   │   ├── index.js                        # React entry point
│   │   ├── routes.js                       # React Router configuration
│   ├── tests/                              # Frontend tests
│   │   ├── testHomePage.js                 # Tests for HomePage
│   │   ├── testTriviaQuiz.js               # Tests for TriviaQuiz component
│   ├── package.json                        # Frontend dependencies
│   ├── .env.example                        # Sample environment variables for frontend
├── docs/                                   # Project documentation
│   ├── README.md                           # Overview and setup instructions
│   ├── INSTALLATION.md                     # Detailed installation guide
│   ├── CONTRIBUTING.md                     # Collaboration guidelines
│   ├── FEATURES.md                         # Detailed list of app features
│   ├── LICENSE                             # License file
├── database.sql                            # SQL schema file for database
├── docker-compose.yml                      # Docker configuration for services
├── Dockerfile                              # Dockerfile for backend
├── Dockerfile.frontend                     # Dockerfile for frontend
└── tests/                                  # Root test directory
    ├── integration/                        # Integration tests
    ├── unit/                               # Unit tests

```

For a detailed breakdown, see the [project tree](#directory-structure).

---

## **Contributing**
We welcome contributions! To get involved:
1. Fork the repository and clone it locally.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push your branch and open a pull request.

For more details, see [CONTRIBUTING.md](docs/CONTRIBUTING.md).

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.
