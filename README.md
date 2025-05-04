# CV Generator MERN Application

A full-stack MERN (MongoDB, Express, React, Node.js) application for creating and managing CVs with authentication.

## Features

- User authentication with role-based access (Candidate/Recruiter)
- CV generation with PDF export
- AWS S3 integration for CV storage
- Candidate profile management
- Recruiter dashboard to view all CVs
- Responsive design

## Tech Stack

- **Frontend**: React, React Bootstrap, React Router
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Authentication**: JWT
- **File Storage**: AWS S3
- **PDF Generation**: PDFMake

## Installation

### Prerequisites

- Node.js (v14+)
- MongoDB
- AWS S3 Bucket (optional)

### Setup

1. Clone the repository:
   ```
   git clone https://github.com/BahriniHoussem001/ProjectMern.git
   cd ProjectMern
   ```

2. Install dependencies:
   ```
   # Install backend dependencies
   cd Backend
   npm install

   # Install frontend dependencies
   cd ../client
   npm install
   ```

3. Environment Variables:
   - Create a `.env` file in the Backend directory based on `.env.example`
   - Fill in your MongoDB connection string and AWS credentials

4. Start the application:
   ```
   # Start backend server
   cd Backend
   npm start

   # Start frontend in a new terminal
   cd client
   npm start
   ```

5. Access the application at `http://localhost:3000`

## Usage

### Candidate Flow
1. Register as a candidate
2. Create your CV by filling out the form
3. View and download your CV from your profile

### Recruiter Flow
1. Register as a recruiter
2. Browse all candidate CVs
3. Download CVs or contact candidates directly

## Project Structure

```
project-root/
├── Backend/                # Backend server
│   ├── middleware/         # Authentication middleware
│   ├── models/             # MongoDB models
│   ├── routes/             # API routes
│   ├── utils/              # Utility functions
│   ├── .env                # Environment variables (not in repo)
│   └── server.js           # Server entry point
├── client/                 # React frontend
│   ├── public/             # Static files
│   ├── src/                # React source code
│   │   ├── components/     # React components
│   │   ├── context/        # Context providers
│   │   └── App.js          # Main App component
└── .gitignore              # Git ignore file
```

## License

This project is licensed under the MIT License.

## Acknowledgements

- [React Bootstrap](https://react-bootstrap.github.io/)
- [PDFMake](http://pdfmake.org/)
- [AWS SDK for JavaScript](https://aws.amazon.com/sdk-for-javascript/)
