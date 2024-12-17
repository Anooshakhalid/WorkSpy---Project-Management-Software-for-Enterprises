# WorkSpy: User and Project Management Tool  

**WorkSpy** is a user and project management tool that streamlines task management, user monitoring, and timesheet reporting with a focus on efficiency and transparency.

---

## Features  

- **Role-Based Access Control**: Secure authentication with user-specific dashboards.  
- **Project and Task Management**: Track project statuses, assign tasks, and monitor progress.  
- **Timesheet Reporting**: Log and visualize weekly working hours, task statuses, and approvals.  
- **Notifications**: Alerts for pending tasks, timesheet reviews, and deadlines.  
- **Charts and Analytics**: Interactive visualizations powered by Chart.js.  

---

## Technologies Used  

- **Backend**: Node.js, Express.js  
- **Database**: MySQL  
- **Frontend**: EJS, HTML, CSS, Chart.js  
- **Authentication**: JSON Web Tokens (JWT) and Express-Session  
- **Encryption**: bcrypt.js  

---

## Installation and Setup  

### Prerequisites  

- Node.js (v14+)  
- MySQL Server (v8+)  
- Git  

### Steps  

1. **Clone Repository**:  
   ```bash  
   git clone https://github.com/Laiba-Iqrar/WorkSpy---User-Project-Management-Tool-for-Enterprises.git 
   cd workspy  
   ```  

2. **Install Dependencies**:  
   ```bash  
   npm install  
   ```  

3. **Configure Environment Variables**:  
   Create a `.env` file:  
   ```env  
   DB_HOST=localhost  
   DB_USER=root  
   DB_PASSWORD=yourpassword  
   DB_NAME=workspy  
   SESSION_SECRET=your_secret_key  
   ```  

4. **Setup Database**:  
   Run the schema file to create tables:  
   ```sql  
   source schema.sql;  
   ```  

5. **Start Server**:  
   ```bash  
   npm start  
   ```  
   Access the application at `http://localhost:3000`.  

---


## Key Routes  

### **Authentication**  

- `POST /login`: Authenticate users and start a session.  
- `GET /logout`: End user session.  

### **Project Management**  

- `GET /projects`: List all projects.  
- `POST /projects`: Create a new project.  
- `PUT /projects/:id`: Update a project.  
- `DELETE /projects/:id`: Delete a project.

### **Reports**  

- `GET /reports`: Fetch task, timesheet, and approval data for charts.  

---

 ## Screenshorts

 - Index page
 - ![Screenshot 2024-11-28 203917](https://github.com/user-attachments/assets/b90f37ad-5330-442f-8590-407351344ba0)


