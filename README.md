# **Food Distribution Management System**

**Food Distribution Management System** is a comprehensive platform designed to combat food insecurity and reduce waste through efficient food donation management. Built with modern web technologies, it facilitates secure and traceable food distribution transactions using OTP-based verification.

## **System Architecture**
[System architecture diagram above shows the interaction between different components]

## **Key Features**
- **Secure Food Donation Management**: End-to-end system for managing food donations and distribution
- **OTP Verification**: Secure validation of donation requests using phone-based OTP
- **Real-time Tracking**: Monitor food distribution status and impact metrics
- **User Authentication**: Secure access for donors, volunteers, and administrators
- **Analytics Dashboard**: Track distribution patterns and impact metrics

## **Technologies Used**
- **Frontend**:
  - **React.js**: UI framework for building interactive interfaces
  - **Tailwind CSS**: Utility-first CSS framework for styling
  - **Recoil**: State management for React applications

- **Backend**:
  - **Node.js**: Server runtime environment
  - **Express.js**: Web application framework
  - **Sinch API**: OTP verification and SMS services
  - **MongoDB**: NoSQL database for data storage

## **Setup and Installation**

### **Prerequisites**
- **Node.js** (v14 or higher)
- **MongoDB** (v4.4 or higher)
- **Sinch API** credentials
- **npm** or **yarn**

### **Installation Steps**

1. **Clone the repository**:
   ```bash
   git clone [repository-url]
   cd food-distribution-system
   ```

2. **Install dependencies**:
   ```bash
   # Install frontend dependencies
   cd client
   npm install

   # Install backend dependencies
   cd ../server
   npm install
   ```

3. **Environment Configuration**:
   Create `.env` files in both client and server directories:

   **Server (.env)**:
   ```plaintext
   MONGODB_URI=your_mongodb_uri
   SINCH_API_KEY=your_sinch_api_key
   SINCH_API_SECRET=your_sinch_api_secret
   JWT_SECRET=your_jwt_secret
   ```

   **Client (.env)**:
   ```plaintext
   REACT_APP_API_URL=http://localhost:5000/api
   ```

4. **Database Setup**:
   ```bash
   # Start MongoDB service
   mongod
   ```

5. **Run the Application**:
   ```bash
   # Start backend server
   cd server
   npm run dev

   # Start frontend application
   cd client
   npm start
   ```

## **API Endpoints**

### **Authentication**
- `POST /api/auth/register`: Register new user
- `POST /api/auth/login`: User login
- `POST /api/auth/verify-otp`: Verify OTP

### **Donations**
- `POST /api/donations`: Create donation
- `GET /api/donations`: List donations
- `GET /api/donations/:id`: Get donation details
- `PUT /api/donations/:id`: Update donation status

### **Distribution**
- `POST /api/distribution`: Record distribution
- `GET /api/distribution/stats`: Get distribution statistics

## **Project Structure**
```
food-distribution-system/
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── state/
│   │   └── services/
│   └── package.json
├── server/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   └── services/
│   └── package.json
└── README.md
```

## **Contributing**
Contributions are welcome! Please feel free to submit a Pull Request. For major changes:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## **License**
This project is licensed under the **MIT License**.

## **Contact**
For any queries regarding the project, please reach out to:
- [Suckaaatit] [nakashmha@gmail.com]
