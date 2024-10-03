
# Laundry Management System @ULaundry

## Project Description

The Laundry Management System is a web application designed for students and laundry personnel in a hostel environment. It provides students with an interface to submit laundry forms, track the status of their clothes, and manage their accounts. The system aims to eliminate boring paperwork and promote a paperless environment, thereby contributing to environmental sustainability. Admin (laundry personnel) can view, sort, and update the status of all laundry forms submitted by the students, making the process efficient and eco-friendly.

## Tech Stack

**Frontend:**
- HTML5
- CSS3
- EJS (Embedded JavaScript)

**Backend:**
- Node.js
- Express.js

**Database:**
- MongoDB
- Mongoose

**Session Management:**
- express-session

## Features

- **Student Authentication & Authorization:**
  - Students can register and log in to the system using their room number, hostel, and password.

- **Laundry Form Submission:**
  - Students can fill in laundry forms specifying the number of different clothing items to be washed.

- **Status Tracking:**
  - Students can view the status of their laundry ("Pending", "Picked", "Washed").

- **Admin Panel:**
  - Admins can view all submitted forms, filter them by date and hostel, and update their status.

- **Cloth Counting:**
  - Admins can view total cloth counts submitted by students on a weekly and monthly basis.

- **Hostel Filtering:**
  - Admins can filter forms based on the hostel, making it easier to manage laundry requests.

- **Account Management:**
  - Students can delete their accounts, which will also remove all their associated laundry forms.

## Installation and Setup

To run the application locally, follow these steps:

### Prerequisites
Make sure you have the following installed:
- Node.js
- MongoDB

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/laundry-management-system.git
   cd laundry-management-system
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory to set environment variables:
   ```plaintext
   PORT=3000
   MONGODB_URI=mongodb+srv://username:password@cluster0.lklbc3z.mongodb.net/laundry?retryWrites=true&w=majority
   SESSION_SECRET=your_secret_key
   ```

4. Start the server:
   ```bash
   npm start
   ```

5. Navigate to the following URLs in your browser:
   - http://localhost:3000 - Home Page
   - http://localhost:3000/signup - Student Signup Page
   - http://localhost:3000/studentlogin - Student Login Page
   - http://localhost:3000/laundrylogin - Admin Login Page
   - http://localhost:3000/dashboard - Student Dashboard
   - http://localhost:3000/admin - Admin Dashboard

## File Structure
```
├── views                  # EJS templates for rendering pages
│   ├── home.ejs           # Home page
│   ├── login.ejs          # Student login page
│   ├── loginadmin.ejs     # Admin login page
│   ├── signup.ejs         # Student signup page
│   ├── form.ejs           # Laundry form submission page
│   ├── dashboard.ejs      # Student dashboard
│   ├── admin.ejs          # Admin dashboard (includes total cloth counts)
├── models                 # Mongoose schema and models
│   ├── user.js            # User schema
│   ├── laundryForm.js     # Laundry form schema
│   ├── laundryPerson.js    # Laundry personnel schema
│   └── clothCount.js      # Schema for tracking cloth counts (total counts)
├── public                 # Static files (CSS, images, etc.)
├── index.js               # Main server file
└── README.md              # Project documentation

```

## Usage
- Students can sign up, log in, and submit laundry forms.
- Admins can log in, view student forms, filter by hostel and date, and update the status.
- Admins can view total cloth counts on a weekly and monthly basis.

## Contributions
Feel free to fork the repository and submit pull requests. Contributions are welcome to add new features or fix bugs!

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
Vansh Nagpal
