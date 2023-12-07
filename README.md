# Workout Tracker - MERN Stack

## Overview

This is a simple single-page workout tracker application built using the MERN stack. The application allows users to track their daily workouts, including details like exercise name, sets, and repetitions.

## Features

- **Track Workouts:** Log different types of exercises, specifying details such as sets, and repetitions.
- **Add Workout Form:** A simple form to add new workout entries.

## Technologies Used

- **Frontend:**
  - React

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (Atlas) for database storage

### Setup

#### Prerequisites

- Node.js and npm installed locally
- MongoDB Atlas account (or a local MongoDB server)

#### Installation

1. Clone the repository:

   ```sh
    git clone https://github.com/yourusername/workout-tracker-mern.git
   ```
2. Navigate to the project directory:
```sh
    cd workout-tracker
```
#### Frontend Installation

1. Navigate to the frontend directory:
```sh
   cd frontend
```
2. Install dependencies:
```sh
npm install
```

3. For Vite Users only:

- If you are using Vite, modify the Vite configuration file (vite.config.js or vite.config.ts) with the following code:
```jsx
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react';

export default defineConfig({
  server: {
    proxy: {
      '/api': 'http://localhost:4000',
    },
  },
  plugins: [react()],
});

```

4. Start the development server:
```sh
npm run dev
```

5. Open your browser and navigate to [http://localhost:5173](http://localhost:5173).

#### Backend Installation

1. Navigate to the backend directory:
```sh
cd backend
```

2. Install dependencies:
```sh 
npm install
```

3. Create a `.env` file in the root directory with the following variables:
```txt
PORT=4000
MONGO_URI=your_mongodb_uri
```

4. Update the "scripts" section in the `package.json` file:
```json
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "node server.js",
    "dev": "nodemon server.js"
  }
```

5. Start the development server:
```sh
npm run dev
```

6. The backend server should be running on [http://localhost:4000](http://localhost:5000/).

#### Task List
- [ ] Add Authentication: Implement user authentication for secure access.
- [ ] Improve UI: Enhance the user interface for a better user experience.

#### Contributing
If you'd like to contribute to this project, please follow these guidelines:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a new Pull Request
