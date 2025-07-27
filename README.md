
# Student Result Management System (SRMS)

A **desktop-based Student Result Management System** for efficiently managing courses, student information, and results, all powered by Python and Tkinter for the GUI, and SQLite for database management.

## ✨ Features

- **User Registration:** Register new users for access control.
- **Dashboard:** View overall statistics—Total Courses, Students, and Results.
- **Course Management:** Add, update, delete, and view course details (name, duration, charges, description).
- **Student Management:** Manage roll number, name, email, gender, DOB, contact, admission date, course, and address.
- **Result Management:** Enter marks by roll number, auto-calculate percentage, manage results.
- **View Results/Reports:** Search and view individual student results.
- **Database Integration:** Uses SQLite for storage, with an initial setup via `create_db.py`.

## 🛠️ Technologies Used

- **Python:** Main programming language.
- **Tkinter:** GUI development.
- **SQLite3:** Local database management.
- **Pillow (PIL):** Image handling in the UI.
- **pymysql:** For optional user registration/auth via external MySQL.

## 📁 Project Structure

```
Student-Result-Management-System/
├── Images/
│   ├── b2.jpg       # Registration Background
│   ├── bg.png       # Dashboard Background
│   ├── c.png        # Clock icon
│   ├── cl.jpg       # Clock face
│   ├── clock_new.png# Clock with hands
│   ├── logo_p.png   # Graduation cap logo
│   ├── register.png # Register button
│   ├── result.jpg   # Result page
│   └── side.png     # Registration side image
├── __pycache__/     # Python cache and compiled files
├── course.py        # Course management module
├── create_db.py     # DB setup script
├── dashboard.py     # Main dashboard module
├── register.py      # User registration logic
├── report.py        # Results viewing/reporting
├── result.py        # Result management logic
└── student.py       # Student information management
```

## ⚙️ Setup and Installation

1. **Clone the Repository:**
   ```
   git clone 
   cd Student-Result-Management-System
   ```

2. **Install Dependencies:**
   ```
   pip install Pillow pymysql
   # tkinter is typically included in Python distributions
   ```

3. **Initialize the Database:**
   ```
   python create_db.py
   ```
   - The `result` table is created automatically when you run `result.py` for the first time.

4. **MySQL (Optional, for Registration):**
   - Edit `register.py` for MySQL settings.
   - Ensure a MySQL server is running (`localhost`, user `root`, empty password, DB `employee2`, table `employee`), or adjust connection details accordingly.

## ▶️ Usage

- **Run the main application:**
  ```
  python dashboard.py
  ```
- **Navigate:** Use dashboard buttons to access Course, Student, Result, and Report modules.
- **Manage Data:** Add, update, delete, and view courses, students, and results records within their respective modules.

---

*For customization and debugging, refer to the individual Python script files for further implementation details.*

## 🔍 Conclusion

The Student Result Management System (SRMS) offers a **robust and user-friendly solution** for efficiently managing student academic data. Leveraging Python with Tkinter for its **intuitive graphical interface** and SQLite for **reliable data storage**, SRMS streamlines critical administrative tasks such as course enrollment, student record keeping, and result processing. This system provides a **centralized and accessible platform** that significantly enhances data management efficiency and accuracy for educational institutions. Its **modular design** allows for straightforward expansion, making it a valuable tool for any academic environment seeking to modernize its record-keeping processes.


