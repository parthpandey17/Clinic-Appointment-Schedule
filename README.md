# 🏥 Clinic Appointment Schedule

A comprehensive web application for managing clinic appointments with separate interfaces for patients and administrators. This full-stack application provides appointment booking, payment processing, and administrative management features.

## ✨ Features

### Patient Portal (Frontend)
- 👤 User registration and authentication
- 📅 Appointment booking with available time slots
- 💳 Secure payment processing (Stripe & Razorpay)
- 📱 Responsive design with modern UI
- 🔔 Real-time notifications
- 📋 Appointment history and management

### Admin Panel
- 🏥 Doctor and clinic management
- 📊 Appointment dashboard and analytics
- 👨‍⚕️ Staff management
- 💰 Payment and billing oversight
- 📈 Reporting and statistics
- ⚙️ System configuration

### Backend API
- 🔐 JWT-based authentication
- 🗄️ MongoDB database integration
- 📤 File upload capabilities (Cloudinary)
- 💸 Payment gateway integration
- 🛡️ Data validation and security
- 🌐 RESTful API endpoints

## 🛠️ Tech Stack

### Frontend & Admin
- **React** 18.3.1 - UI library
- **Vite** - Build tool and development server
- **React Router DOM** - Client-side routing
- **Tailwind CSS** - Utility-first CSS framework
- **Axios** - HTTP client
- **React Toastify** - Notification system

### Backend
- **Node.js** with **Express.js** - Server framework
- **MongoDB** with **Mongoose** - Database and ODM
- **JWT** - Authentication tokens
- **bcrypt** - Password hashing
- **Cloudinary** - Image storage and management
- **Stripe & Razorpay** - Payment processing
- **Multer** - File upload handling
- **CORS** - Cross-origin resource sharing

## 📁 Project Structure

```
clinic-appointment-schedule/
├── frontend/          # Patient-facing React application
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
├── backend/           # Node.js Express API server
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── server.js
│   └── package.json
├── admin/             # Admin panel React application
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
└── README.md
```

## 🚀 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or Atlas)
- npm or yarn package manager

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/clinic-appointment-schedule.git
cd clinic-appointment-schedule
```

### 2. Backend Setup
```bash
cd backend
npm install

# Create .env file with your configuration
cp .env.example .env
# Edit .env with your database URL, JWT secret, payment keys, etc.

npm run server  # Development with nodemon
# or
npm start      # Production
```

### 3. Frontend Setup
```bash
cd frontend
npm install
npm run dev    # Development server
# or
npm run build  # Production build
```

### 4. Admin Panel Setup
```bash
cd admin
npm install
npm run dev    # Development server
# or
npm run build  # Production build
```

## ⚙️ Environment Variables

Create a `.env` file in the backend directory:

```env
# Database
MONGODB_URI=your_mongodb_connection_string

# JWT
JWT_SECRET=your_jwt_secret_key

# Cloudinary (for image uploads)
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Payment Gateways
STRIPE_SECRET_KEY=your_stripe_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret

# Server
PORT=5000
NODE_ENV=development
```

## 🎯 Usage

1. **Start the Backend Server**
   ```bash
   cd backend && npm run server
   ```

2. **Start the Frontend Application**
   ```bash
   cd frontend && npm run dev
   ```

3. **Start the Admin Panel**
   ```bash
   cd admin && npm run dev
   ```

4. **Access the Applications**
   - Frontend (Patient Portal): `http://localhost:5173`
   - Admin Panel: `http://localhost:5174`
   - Backend API: `http://localhost:5000`

## 📚 API Endpoints

The backend provides RESTful API endpoints for:
- `/api/auth` - Authentication (login, register, logout)
- `/api/appointments` - Appointment management
- `/api/doctors` - Doctor information
- `/api/patients` - Patient profiles
- `/api/payments` - Payment processing
- `/api/admin` - Administrative functions

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🛟 Support

If you encounter any issues or have questions, please:
1. Check the existing issues on GitHub
2. Create a new issue with detailed information
3. Contact the development team

## 🙏 Acknowledgments

- Thanks to all contributors who have helped build this project
- Built with modern web technologies and best practices
- Designed with user experience and security in mind

---

**Made with ❤️ for better healthcare management**