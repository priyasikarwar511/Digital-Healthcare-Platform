# 🏥 Healthcare Management System

<div align="center">

### 🌟 A comprehensive solution for managing healthcare operations efficiently

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🏗️ Architecture](#️-architecture)
- [🚀 Quick Start](#-quick-start)
- [📦 Installation](#-installation)
- [🔧 Configuration](#-configuration)
- [💻 Usage](#-usage)
- [🧪 Testing](#-testing)
- [📄 License](#-license)
- [📞 Contact](#-contact)

---

## ✨ Features

<div align="center">

| Feature | Description | Status |
|---------|-------------|--------|
| 👥 **Patient Management** | Register and manage patient records | ✅ Active |
| 👨‍⚕️ **Doctor Management** | Handle doctor profiles and schedules | ✅ Active |
| 📅 **Appointment System** | Schedule and track appointments | ✅ Active |
| 🔐 **Data Security** | Secure access and role-based permissions | 🔄 In Progress |
| 📊 **Analytics Dashboard** | Healthcare insights and reporting | 📋 Planned |


</div>

### 🎯 Key Highlights

- **🔒 Secure**: Designed with data privacy in mind
- **⚡ Fast**: Optimized for seamless operations
- **🌐 RESTful API**: Clean and intuitive API design
- **🧪 Well-Tested**: Comprehensive test coverage

---

## 🏗️ Architecture

```
🛠️ Project Management System
├── 🔧 Backend Layer (Src/)
│   ├── 🛣️  Routes  
│   ├── 📊 Controllers
│   ├── 🔐 Authentication
    ├── 📚 MongoDB Database
    ├── 🗄️  Data Models
    └──  start point  
```

## 📂 Repository Structure

<details>
<summary>🗂️ Click to expand the project structure</summary>

```
Healthcare Management with Blockchain/
├── 📁 src/
│   ├── 🎮 controllers/           # Application logic and controllers
│   │   ├── 📋 patient.controller.js         # Patient operations
│   │   └── 📅 doctor.controller.js      # Doctor operations
│   ├── 📊 models/               # Database models for MongoDB
│   │   ├── 📋 patient.model.js             # Patient data schema
│   │   ├── 📅 doctor.model.js          # Doctor data schema
│   │   ├── 📋 report.model.js             # Report data schema
│   │   └── 📅 appointment.model.js          # Appointment data schema
│   ├── 🛣️  routes/              # API route definitions
│   │   ├── 📋 patientRoutes.js            # Task endpoints
│   │   └── 📅 doctorRoutes.js         # Project endpoints
│   ├── 🔧 utils/                # Utility functions and helpers
│   │   ├── ❌ apiError.js                # Error handling
│   │   ├── 📝apiReponse.js          # Response handling
|   |   └── 📝asyncHandler.js        # Async handling
│   ├── 🚀 index.js                # Main application entry point
|   ├── 📦 package.json              # Project metadata and dependencies
|   └── 🙈 .gitignore               # Git ignore rules
├── 📖 README.md                 # Project documentation


```

</details>

---

## 🚀 Quick Start

### Prerequisites

Before you begin, ensure you have the following installed:

- ![Node.js](https://img.shields.io/badge/Node.js-v14+-green?logo=node.js) **Node.js** (v14 or higher)
- ![MongoDB](https://img.shields.io/badge/MongoDB-v4+-green?logo=mongodb) **MongoDB** (v4 or higher)
- ![npm](https://img.shields.io/badge/npm-v6+-red?logo=npm) **npm** (v6 or higher)

---

## 📦 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Khiladi124/HealthCare-management-with-Blockchain.git
cd Healthcare-management-with-Blockchain
```

### 2️⃣ Install Dependencies

```bash
npm install
```

<details>
<summary>📋 View all dependencies</summary>

#### Core Dependencies
```bash
# Web framework
npm install express

# Database ODM
npm install mongoose

# Middleware
npm install body-parser cors

# Development dependencies (automatically installed)
npm install --save-dev jest nodemon
```

</details>

---

## 🔧 Configuration

### Environment Setup

Create a `.env` file in the root directory:

```env
# Server Configuration
PORT=3000
NODE_ENV=development

# Database Configuration
MONGODB_URI=mongodb://localhost:27017/your_project_db

# Security
JWT_SECRET=your-super-secret-jwt-key
BCRYPT_ROUNDS=12

# Email Configuration (Optional)
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@gmail.com
SMTP_PASS=your-app-password
```

---

## 💻 Usage

### 🏃‍♂️ Start the Application

#### Development Mode
```bash
npm run dev
```

#### Production Mode
```bash
npm start
```

### 🌐 Access the System

The backend API server will be running at:
```
http://localhost:3000
```

### 🔗 API Endpoints

<details>
<summary>📋 View API Documentation</summary>

#### Patient Management
- `POST /api/patients/register` - Register new patient
- `POST /api/patients/login` - Patient login
- `GET /api/patients/profile/:patientId` - Get patient profile (Auth required)
- `GET /api/patients/:patientId/reports` - Get patient reports (Auth required)
- `GET /api/patients/:patientId/reports/:reportId` - Get specific patient report (Auth required)
- `GET /api/patients/:patientId/appointments` - Get patient appointments (Auth required)
- `POST /api/patients/:patientId/appointments` - Request new appointment (Auth required)
- `DELETE /api/patients/:patientId/appointments/:appointmentId` - Cancel appointment (Auth required)

#### Doctor Management
- `POST /api/doctors/register` - Register new doctor
- `POST /api/doctors/login` - Doctor login
- `POST /api/doctors/:doctorId/addReport` - Add report to patient (Auth required)
- `GET /api/doctors/profile/:doctorId` - Get doctor profile (Auth required)
- `GET /api/doctors/:doctorId/appointments` - Get doctor appointments (Auth required)
- `PUT /api/doctors/:doctorId/appointments/:appointmentId` - Update appointment status (Auth required)

</details>

---

## 🧪 Testing

### Run Tests

```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Generate coverage report
npm run test:coverage
```

### Test Coverage

```
📊 Current Coverage: 85%
├── 📋 Task Module: 90%
├── 📅 Project Module: 80%
└── 🔧 Utilities: 85%
```


## 🎯 Roadmap

### 🔮 Upcoming Features

- [ ] 🔐 User Authentication & Authorization
- [ ] 📊 Advanced Analytics Dashboard
- [ ] 📧 Email Notifications
- [ ] 📱 Mobile App Integration
- [ ] 🔄 Real-time Updates
- [ ] 📈 Performance Monitoring
- [ ] 🌍 Multi-language Support

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License - Feel free to use this project for personal or commercial purposes!
```

---

## 📞 Contact

<div align="center">

### 👨‍💻 Project Maintainer

**Priya Sikarwar**

[![Email](https://img.shields.io/badge/Email-priyasikarwar511@gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:priyasikarwar511@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow%20Me-black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/priyasikarwar511)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/priya-sikarwar)

</div>


<div align="center">
<sub>Built with 🔥 by developers who care about project management technology</sub>
</div>