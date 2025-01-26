# Resume Builder Application

### **Overview**
The Resume Builder application is a professional tool designed to help users create, customize, and manage resumes easily. Built using the **MERN stack (MongoDB, Express.js, React, Node.js)**, the application provides a responsive user interface and robust backend, ensuring a seamless experience for users across devices.

---

## **Features**
- **User Registration & Login**: Secure authentication to protect user data.  
- **Dynamic Resume Templates**: Users can choose and customize templates dynamically.  
- **Data Persistence**: User details and resume data are stored securely in MongoDB.  
- **Responsive Design**: Ensures compatibility across various devices (mobile, tablet, desktop).  
- **RESTful APIs**: Backend services handle user and resume data efficiently.  

---

## **Tech Stack**

### 1. **Front-End**:
- React.js: For building an intuitive and interactive UI.  
- CSS: Ensures responsiveness and appealing design.  

### 2. **Back-End**:
- Node.js: Handles server-side logic.  
- Express.js: Simplifies API creation and routing.  

### 3. **Database**:
- MongoDB: For storing user data and resume details.  

### 4. **Other Tools**:
- Axios: For API calls between the front-end and back-end.  
- bcrypt: For secure password hashing.  

---

## **Installation and Setup**

Follow these steps to set up and run the project locally:

### 1. **Prerequisites**:
- Node.js installed on your system.  
- MongoDB installed or access to a MongoDB cloud instance (e.g., MongoDB Atlas).  
- Git installed on your system.  

### 2. **Clone the Repository**:
```bash
git clone <repository-url>
cd ResumeBuilder03-master
```

### 3. **Backend Setup**:
1. Navigate to the `server` directory:
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables in a `.env` file:
   ```env
   PORT=5000
   MONGO_URI=<your-mongodb-uri>
  
   ```
4. Start the server:
   ```bash
   npm start
   ```

### 4. **Frontend Setup**:
1. Navigate to the `client` directory:
   ```bash
   cd client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm start
   ```

### 5. **Access the Application**:
Once both servers are running:  
- Open the browser and navigate to: `http://localhost:3000`

---

## **Project Architecture**
```plaintext
Resume Builder
├── client                 # Front-end (React)  
│   ├── public             # Static files  
│   ├── src                # Source files  
│       ├── components     # Reusable React components  
│       ├── pages          # Application pages (e.g., Home, Templates)  
│       ├── App.js         # Main React component  
│       └── index.js       # Entry point  
├── server                 # Back-end (Node.js, Express.js)  
│   ├── models             # Database schemas  
│   ├── routes             # API routes  
│   ├── server.js          # Server configuration  
│   └── .env               # Environment variables  
└── README.md              # Documentation
```

---

## **Key Functionalities**

### 1. **Authentication**
- Users can register and log in securely.  
- Passwords are hashed using bcrypt before being stored in the database.  

### 2. **Resume Customization**
- Users can input personal, educational, and professional details.  
- Multiple templates are available for dynamic resume generation.  

### 3. **Data Storage and Retrieval**
- User profiles and resume data are stored in MongoDB.  
- REST APIs handle CRUD operations efficiently.  

---

## **API Endpoints**

### **Authentication**
1. **Register**:  
   - **URL**: `/api/user/register`  
   - **Method**: POST  
   - **Request Body**:  
     ```json
     {
       "name": "John Doe",
       "email": "john.doe@example.com",
       "password": "securepassword"
     }
     ```  

2. **Login**:  
   - **URL**: `/api/user/login`  
   - **Method**: POST  

### **Resume Management**
1. **Save Resume**:  
   - **URL**: `/api/resume/save`  
   - **Method**: POST  

2. **Fetch Resume**:  
   - **URL**: `/api/resume/:id`  
   - **Method**: GET  

---

## **Future Enhancements**
- Add more resume templates for better customization.  
- Integrate drag-and-drop functionality for rearranging resume sections.  
- Add social media integration to fetch LinkedIn profiles.  
- Deploy the application on cloud platforms like AWS or Heroku.  

---

## **Contributing**
Contributions are welcome! Follow these steps:  
1. Fork the repository.  
2. Create a feature branch (`git checkout -b feature-name`).  
3. Commit changes (`git commit -m "Add feature"`).  
4. Push to the branch (`git push origin feature-name`).  
5. Open a pull request.  

---


