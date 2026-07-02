<div align="center">

# 🚀 CivicFix

### AI-Powered Infrastructure Issue Reporting Platform

Detect, report, and track civic infrastructure issues using Machine Learning, automatic location detection, and an administrator dashboard.

</div>

---

# 📖 Overview

CivicFix is an AI-powered infrastructure issue reporting platform developed during a hackathon to simplify reporting civic problems such as potholes, road cracks, water leakage, and damaged streetlights.

Users can upload an image of an issue, automatically detect their current location, and submit a report. The uploaded image is classified using a machine learning model, while complaint details are stored in MongoDB and images are securely uploaded to Cloudinary.

Administrators can review reports through a dedicated dashboard, update complaint statuses, and monitor recently submitted issues.

---

# ✨ Features

- 📸 Upload infrastructure issue images
- 🤖 AI-powered image classification
- 📍 Automatic GPS location detection
- 🗺 Reverse geocoding for Area, District & Pincode
- ☁ Cloudinary image storage
- 🗄 MongoDB integration
- 👨‍💼 Secure Admin Login
- 📊 Admin Dashboard
- 🔄 Real-time complaint status updates
- 📋 Recent Reports section
- 📱 Responsive user interface

---

# 🎯 Supported Issue Categories

- 🛣 Potholes
- 🚧 Road Cracks
- 💡 Street Light Faults
- 💧 Water Leakage

---

# 🛠 Tech Stack

## Frontend

- HTML5
- CSS3
- JavaScript

## Backend

- Node.js
- Express.js

## Database

- MongoDB

## Machine Learning

- Python
- PyTorch
- TorchVision
- Pillow

## Cloud Storage

- Cloudinary

---

# 📂 Project Structure

```text
CivicFix/
│
├── backend/
│   ├── ai/
│   │   └── requirements.txt
│   └── ...
│
├── frontend/
├── .gitignore
└── README.md
```

---

# 🚀 Getting Started

Clone the repository

```bash
git clone https://github.com/Archana7code/CivicFix.git
```

Move into the project directory

```bash
cd CivicFix
```

Install backend dependencies

```bash
npm install
```

Install Python dependencies

```bash
cd backend/ai
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file inside the **backend** directory.

```env
MONGODB_URI=your_mongodb_connection_string

CLOUDINARY_URL=your_cloudinary_url

JWT_SECRET=your_secure_jwt_secret
```

---

# ⚠️ Important

This repository does **not** include sensitive credentials.

To run the complete project, configure your own:

- MongoDB Database
- Cloudinary Account

---

# 📸 Screenshots

## 🏠 Home Page

<img width="1891" height="876" alt="image" src="https://github.com/user-attachments/assets/54800137-22e5-4189-b713-3a0ea1af506f" />

---

## 📤 Report Issue

<img width="1882" height="878" alt="image" src="https://github.com/user-attachments/assets/7fc1131e-28cf-4d9d-8d5d-d62806231d72" />

---

## 👨‍💼 Admin Dashboard

<img width="1910" height="872" alt="image" src="https://github.com/user-attachments/assets/357123ee-f2af-4721-8f2f-5d19502cffb3" />


---

# 👨‍💻 My Contributions

This project was originally developed during a hackathon by a team of three members.

My contributions include:

- Designed and trained the complete machine learning model for infrastructure issue classification.
- Contributed to frontend development and user interface implementation.
- Assisted in backend development and API integration.
- Participated in testing and deployment during the hackathon.

---

# 🚀 Future Improvements

- Integrate government complaint portal APIs
- GIS-based map visualization of reported issues
- AI-powered severity prediction
- Push notifications for complaint updates
- Mobile application
- Advanced analytics dashboard
- Multi-language support

---

# 📌 Project Status

The project demonstrates the complete workflow of AI-assisted civic issue reporting, including image classification, automatic location detection, complaint submission, and administrator management.

Backend services require environment configuration before deployment.

---

# 👨‍💻 Developer

**Archana Verma**

GitHub: https://github.com/Archana7code

💼 LinkedIn: https://www.linkedin.com/in/archana-verma-287b3a328/

---

## ⭐ Support

If you found this project interesting, consider giving it a ⭐ on GitHub.
