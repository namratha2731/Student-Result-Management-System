Student Result Management System (SRMS)
This project is a desktop-based Student Result Management System built using Python with Tkinter for the graphical user interface and SQLite for database management. It provides functionalities for managing courses, student details, adding and viewing results, and user registration.

✨ Features
User Registration: Allows new users to register and manage access to the system.

Dashboard: A central dashboard displaying overall statistics (Total Courses, Total Students, Total Results).

Course Management: Add, update, delete, and view course details such as course name, duration, charges, and description.

Student Management: Manage student information including roll number, name, email, gender, date of birth, contact, admission date, course, and address details.

Result Management: Add student results by selecting a student's roll number, entering marks obtained, and full marks. Calculates percentage automatically.

View Results/Reports: Search and view individual student results.

Database Integration: Uses SQLite for local data storage, with a create_db.py script for initial setup.

🛠️ Technologies Used
Python: Core programming language.

Tkinter: For building the graphical user interface (GUI).

SQLite3: For the local database management system.

Pillow (PIL): For image processing and handling within the Tkinter application.

pymysql: Used in the registration module for connecting to an external MySQL database for user authentication (if configured).

📁 Project Structure
Student-Result-Management-System/
├── Images/
│   ├── b2.jpg                 # Background image for registration
│   ├── bg.png                 # Background image for dashboard
│   ├── c.png                  # Clock image
│   ├── cl.jpg                 # Clock face image
│   ├── clock_new.png          # Clock image with hands
│   ├── logo_p.png             # Project logo (graduation cap)
│   ├── register.png           # Register button image
│   ├── result.jpg             # Result page image
│   └── side.png               # Side image for registration
├── __pycache__/             # Python cache files
│   ├── course.cpython-310.pyc
│   ├── db.db                  # SQLite database file (created on run)
│   ├── report.cpython-310.pyc
│   ├── result.cpython-310.pyc
│   └── student.cpython-310.pyc
├── course.py                # Module for managing course details
├── create_db.py             # Script to initialize the SQLite database
├── dashboard.py             # Main application dashboard and menu
├── register.py              # User registration module
├── report.py                # Module for viewing student results
├── result.py                # Module for adding student results
└── student.py               # Module for managing student details
⚙️ Setup and Installation
Clone the repository:

Bash

git clone <repository_url>
cd Student-Result-Management-System
Install dependencies:
This project requires tkinter, Pillow, and pymysql. tkinter is usually included with Python installations.

Bash

pip install Pillow pymysql
Initialize the database:
Run the create_db.py script to set up the necessary SQLite tables (course and student tables). The result table is created when result.py is run for the first time.

Bash

python create_db.py
Database Configuration for Registration (Optional):
The register.py module attempts to connect to a MySQL database at localhost with user root and an empty password for user registration. If you wish to use this feature, ensure you have a MySQL server running and a database named employee2 with a table named employee for user credentials, or modify the pymysql.connect line in register.py to match your database configuration.

▶️ Usage
Start the application:
Run the dashboard.py file to launch the main application.

Bash

python dashboard.py
Navigate through menus:
The dashboard provides buttons to access different modules: Course, Student, Result, and View Student Results.

Manage Data:
Use the respective modules to add, update, delete, and view course, student, and result details.
