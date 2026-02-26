# 🤖 AI Resume Builder

A modern **AI-powered resume builder application** that helps users create professional, ATS-friendly resumes effortlessly.  
Built with a **MERN stack**, this application uses AI to generate optimized resume content, manage user data securely, and export resumes in a polished format.

## 🚀 Features

- **AI Resume Generation**: Smart AI-generated summaries, skills, and experience
- **ATS-Friendly Resumes**: Optimized formatting for applicant tracking systems
- **Modern UI**: Fast and responsive interface built with React + Vite
- **Multiple Resume Sections**:
  - Personal Details
  - Summary
  - Skills
  - Experience
  - Projects
  - Education
- **PDF Export**: Download resumes in a professional PDF format
- **Secure Authentication**: JWT-based user authentication
- **Scalable Backend**: Modular Node.js + Express architecture
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Dockerized**: Easy setup and deployment with Docker

## 🏗️ Architecture

### Backend (`server/`)

- **Node.js + Express** REST API
- **MongoDB** for data storage
- **Mongoose** for database modeling
- **JWT Authentication**
- **AI API Integration** for resume content generation

### Frontend (`client/`)

- **React.js** with **Vite**
- **JavaScript**
- **Axios** for API communication
- **Modern component-based UI**
- **Environment-based configuration**

---

## 📋 Prerequisites

Before running the project, make sure you have:

- Node.js (v18+ recommended)
- npm or yarn
- MongoDB (local or Atlas)
- OpenAI API account
- Docker (optional)

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/AI-CVForge.git
cd AI-CVForge
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd server
```

Install dependencies:

```bash
npm install
```

Create environment file by copying the example:

```bash
cp .env.example .env
```

Configure your `.env` file with the following keys:

```env
# Get credentials - Get these from your service providers
JWT_SECRET=your_jwt_secret_here
MONGODB_URI=your_mongodb_connection_string_here
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key_here
OPENAI_API_KEY=your_openai_api_key_here
OPENAI_BASE_URL=your_openai_base_url_here
OPENAI_MODEL=gemini-2.5-flash

# OpenAI API key - Get from https://platform.openai.com/api-keys
OPENAI_API_KEY=your_openai_api_key_here
```

### 3. Frontend Setup

Navigate to the frontend directory:

```bash
cd client
```

Install dependencies:

```bash
npm install
```

Create environment file:

```bash
cp .env.example .env
```

Configure your `.env` file:

```env
# Backend URL
VITE_BACKEND_URL=http://localhost:3000
```

## 🚀 Running the Application

### Start the Backend Server

```bash
cd server
npm run server
```

The backend will run on `http://localhost:3000`

### Start the Frontend Application

```bash
cd client
npm run dev
```

The frontend will run on `http://localhost:5173`

### Starting with Docker

Make sure you have Docker installed and running. Then, from the root directory:

```bash
docker-compose up
```
This will start both the backend and frontend services in Docker containers.

# 🎨 UI Components

The frontend uses modern UI components built with:

- **Radix UI**: Accessible component primitives
- **Tailwind CSS**: Utility-first CSS framework
- **shadcn/ui**: Beautiful, customizable components
- **Lucide React**: Modern icon library

## 🔒 Security Features

- **JWT Authentication**: Secure token-based authentication
- **Environment Variables**: Sensitive data protection
- **CORS Configuration**: Cross-origin request security
- **Token Expiration**: Automatic token refresh system
- **Input Validation**: Server-side validation for all requests

## 🚀 Deployment

### Backend Deployment

1. Set environment variables on your hosting platform
2. Run `npm run start` for production
3. Ensure PORT is configured (defaults to 3000)

### Frontend Deployment

1. Run `npm run build` to create production build
2. Deploy the `dist` folder to your static hosting service
3. Configure environment variables for production

## 🛠️ Development

### Backend Development

```bash
cd server
npm run server  # Starts with nodemon for auto-reload
```

### Frontend Development

```bash
cd client
npm run dev  # Starts Vite dev server
```

### Building for Production

```bash
# Backend
cd server
npm run start

# Frontend
cd client
npm run build
```

## 📚 Technologies Used

### Backend

- **Node.js** - Runtime environment
- **Express** - Web framework
- **OpenAI** - AI language model
- **CORS** - Cross-origin resource sharing
- **Mongoose** - MongoDB object modeling
- **JWT** - Authentication
- **ImageKit** - Image upload and management
- **Docker** - Containerization

### Frontend

- **React** - UI library
- **JavaScript** - Programming language
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **Radix UI** - Accessible components
- **React Router** - Navigation
- **Lucide React** - Icons
- **Docker** - Containerization

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License.

## 🆘 Support

If you face any issues or have suggestions:

- Open an issue in this repository
- Share feedback to improve the project

---

Built with ❤️ using MERN stack and AI technologies.
