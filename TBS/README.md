# Tropical Baking Sweets - E-commerce & Landing Page

A full-stack web application for bakery businesses that includes an e-commerce platform, content management system (CMS), and responsive landing page design.

## 🍰 Features

### Customer Features
- Browse bakery products with detailed descriptions and prices
- Place orders through a shopping cart system
- Contact form for custom orders and inquiries
- Image gallery of bakery products
- Responsive design for mobile and desktop

### Admin Features
- Content Management System (CMS) for:
  - Product management (add/edit/delete)
  - Order management and tracking
  - Image upload and gallery management
  - Content editing for landing page
- Dashboard with sales analytics
- Order notification system

## 🛠 Tech Stack
- **Frontend**: React.js, Material-UI
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Containerization**: Docker
- **Image Storage**: Local storage with backup system

## 📋 Prerequisites
- Node.js (v16 or higher)
- Docker and Docker Compose
- MongoDB
- Git

## 🚀 Getting Started

### Local Development Setup
1. Clone this repository:

```bash
git clone https://github.com/yourusername/tropical-baking-sweets.git
cd tropical-baking-sweets
```

2. Set up environment variables:

```bash
# For Backend
cp Server/.env.example Server/.env
# For Frontend
cp client/.env.example client/.env
```

3. Configure your environment variables in both .env files

4. Run with Docker:
```bash
docker-compose up --build
```

### Manual Setup (Without Docker)
1. Install Backend Dependencies:
```bash
cd Server
npm install
npm start
```

2. Install Frontend Dependencies:
```bash
cd client
npm install
npm start
```

## 📁 Project Structure
```
tropical-baking-sweets/
├── client/                 # React frontend
│   ├── src/               # Source files
│   ├── public/            # Public assets
│   └── package.json       # Frontend dependencies
├── Server/                # Node.js backend
│   ├── controllers/       # Request handlers
│   ├── models/           # Database models
│   ├── routes/           # API routes
│   └── package.json      # Backend dependencies
├── Uploads/              # Media storage
└── docker-compose.yml    # Docker configuration
```

## 🔧 Configuration

### Required Environment Variables
#### Backend (.env)
- `MONGODB_URI`: MongoDB connection string
- `PORT`: Server port (default: 8080)
- `FRONTEND_URL`: Frontend application URL
- `JWT_SECRET`: Secret for JWT authentication

#### Frontend (.env)
- `REACT_APP_API_URL`: Backend API URL
- `REACT_APP_SITE_TITLE`: Site title

## 📱 Available Scripts

### Frontend
- `npm start`: Run development server
- `npm build`: Build for production
- `npm test`: Run tests
- `npm run eject`: Eject from Create React App

### Backend
- `npm start`: Start the server
- `npm run dev`: Run with nodemon for development

## 🔒 Security
- All sensitive data must be stored in .env files
- JWT authentication for admin routes
- Input validation and sanitization
- File upload restrictions
- CORS configuration

## 🤝 Contributing
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support
For support, send me a discord msg [@brandonmarriott] or open an issue in the repository.

## 🙏 Acknowledgments
- Create React App
- Material-UI
- Express.js
- MongoDB
