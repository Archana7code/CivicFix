<div align="center">

# 🚀 CivicFix

### AI-Powered Civic Infrastructure Issue Reporting Platform

Detect, report, and manage civic infrastructure issues using Machine Learning, automatic location detection, and an administrator dashboard.

</div>

---

# 📖 Overview

CivicFix is an AI-powered web application that enables users to report civic infrastructure issues such as potholes, road cracks, broken streetlights, and water leaks.

Users can upload an image of an issue, automatically capture their current location, and submit a complaint. The uploaded image is classified using a **fine-tuned ResNet18 image classification model built with PyTorch**, while complaint information is stored in MongoDB and uploaded images are securely stored using Cloudinary.

Administrators can securely log in, review submitted complaints, update their status, and monitor recently reported issues through an intuitive dashboard.

> **Note:** The project was initially developed during a hackathon by a team of three members and later improved with additional refinements.

---

# ✨ Features

- 📸 Upload infrastructure issue images
- 🤖 AI-powered image classification using Transfer Learning (ResNet18)
- 📍 Automatic GPS location detection
- 🗺 Reverse geocoding (Area, District & Pincode)
- ☁ Secure image upload and storage using Cloudinary
- 🗄 MongoDB database integration
- 👨‍💼 Secure Admin Authentication (JWT)
- 📊 Admin Dashboard for complaint management
- 🔄 Complaint status updates
- 📋 Recent Reports section
- 📱 Responsive user interface

---

# 🎯 Supported Issue Categories

- 🛣 Potholes
- 🚧 Road Cracks
- 💡 Broken Streetlights
- 💧 Water Leakage

---

# 🏗 System Architecture

```text
              User
                │
                ▼
         Upload Image
                │
                ▼
      Frontend (HTML/CSS/JS)
                │
                ▼
      Node.js + Express Backend
      │           │            │
      │           │            │
      ▼           ▼            ▼
 Cloudinary    MongoDB     Python (PyTorch)
                              │
                              ▼
                 Fine-tuned ResNet18 Model
                              │
                              ▼
                     Predicted Issue Type
```

---

# 🤖 Machine Learning Workflow

```text
Training Images
       │
       ▼
Resize & Normalize Images
       │
       ▼
Fine-tune Pre-trained ResNet18
       │
       ▼
Save Trained Model (.pth)
       │
       ▼
User Uploads Image
       │
       ▼
Load Model
       │
       ▼
Predict Issue Category
       │
       ▼
Store Complaint & Display Result
```

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
- Transfer Learning (ResNet18)

## Cloud Storage

- Cloudinary

---

# 📂 Project Structure

```text
CivicFix/
│
├── backend/
│   ├── ai/
│   │   ├── train.py
│   │   ├── detectIssue.py
│   │   ├── utils.py
│   │   ├── requirements.txt
│   │   └── model/
│   │       └── model.pth
│   │
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── server.js
│   └── package.json
│
├── frontend/
│
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

Install Node.js dependencies

```bash
npm install
```

Install Python dependencies

```bash
cd backend/ai
pip install -r requirements.txt
```

Start the backend server

```bash
npm start
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

Sensitive credentials are **not included** in this repository.

Configure your own:

- MongoDB Database
- Cloudinary Account
- JWT Secret

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

- Designed and implemented the machine learning pipeline for infrastructure issue classification.
- Fine-tuned a pre-trained ResNet18 image classification model using PyTorch.
- Integrated the ML model into the backend for automated issue prediction.
- Contributed to frontend UI development and user experience improvements.
- Assisted in backend API development and MongoDB integration.
- Participated in testing and deployment during the hackathon.


---

# 🚀 Future Improvements

- Government complaint portal integration
- GIS-based map visualization
- AI-powered issue severity prediction
- Email and push notifications
- Mobile application
- Advanced analytics dashboard
- Multi-language support

---

# 📌 Project Status

CivicFix successfully demonstrates the complete workflow of AI-assisted civic issue reporting, including image classification, automatic location detection, complaint submission, and administrator management.

Deployment requires configuring environment variables for MongoDB, Cloudinary, and JWT authentication.

---

# 👨‍💻 Developer

**Archana Verma**

GitHub: https://github.com/Archana7code

LinkedIn: https://www.linkedin.com/in/archana-verma-287b3a328/

---

## ⭐ Support

If you found this project helpful or interesting, consider giving it a ⭐ on GitHub.