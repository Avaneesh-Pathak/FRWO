# 🧠 Face Recognition Attendance System

An intelligent **Face Recognition Attendance System** built using **Python**, **Django**, and **OpenCV**, designed to automate employee attendance through real-time face detection and recognition.  
This system eliminates manual entry errors and ensures a secure, efficient, and contactless attendance process.

---

## 🚀 Features

- 🧍‍♂️ **Employee Registration & Management**
- 👁️ **Real-Time Face Detection & Recognition**
- ⏰ **Automatic Attendance Marking**
- 📊 **Admin Dashboard with Analytics**
- 📅 **Daily, Weekly & Monthly Attendance Reports**
- 🔒 **Role-Based Authentication (Admin / Employee)**
- 💻 **Modern Web UI with Bootstrap**
- 🌐 **Live Attendance Summary via API**

---

## 🛠️ Installation

Follow the steps below to set up the project on your local machine:

### 1️⃣ Clone the Repository
```bash
https://github.com/Avaneesh-Pathak/FRWO.git

```
2️⃣ Navigate to the Project Directory
```bash
cd facial_attendance
```
3️⃣ Create a Virtual Environment
```bash
python -m venv venv
# activate venv
venv\Scripts\activate
```
4️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```
5️⃣ Apply Database Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```
6️⃣ Create a Superuser (Admin Account)
```bash
python manage.py createsuperuser
```

7️⃣ Run the Development Server
```bash
python manage.py runserver
```
Now open your browser and go to:
```bash
http://127.0.0.1:8000/
```
8️⃣ Access the Admin Panel
```bash
http://127.0.0.1:8000/admin/
```

✅ Optional (Face Recognition Setup)

Make sure the following libraries are installed:
```bash
pip install opencv-python face-recognition dlib numpy
```


Also, ensure your system has a working camera.


## 🧩 Project Structure

```bash
facial_attendance/
│
├── core/                   # Main app (formerly attendance_app)
│   ├── models.py           # Employee & Attendance models
│   ├── views.py            # Logic for attendance and dashboard
│   ├── urls.py
│   ├── templates/
│   │   ├── dashboard.html
│   │   ├── kiosk.html
│   │   └── ...
│   └── static/
│       ├── js/
│       ├── css/
│       └── sounds/
│
├── facial_attendance/      # Project settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── manage.py
├── requirements.txt
└── README.md
```

## ❓ Troubleshooting

### Common Issues

- **dlib installation fails**:
  - Ensure you have CMake installed. On Windows, install Visual Studio with C++ build tools.
  - Try installing the pre-built wheel manually if pip fails.

- **Camera not detected**:
  - Check if another application is using the camera.
  - Verify OpenCV can access index 0 (default camera).

- **Migrations not applying**:
  - Delete `db.sqlite3` and run migrations again if you face conflicts.
  - Ensure `makemigrations` is run before `migrate`.



## 💡 Usage

- 👨‍💼 **Admin** can add employees, view attendance reports, and monitor real-time stats.  
- 🧑‍💻 **Employees** can mark attendance automatically by standing in front of the camera.  
- 🕒 The system records **check-in** and **check-out** times along with a **confidence score** for each recognition event.  
- 📊 Attendance data is updated in real time and can be filtered by **date, week, or month**.

---

## 🧮 Tech Stack

| Component            | Technology                     |
| -------------------- | ------------------------------ |
| **Frontend**         | HTML5, CSS3, Bootstrap 5       |
| **Backend**          | Django 4+, Python 3.10+        |
| **Database**         | SQLite / PostgreSQL            |
| **Face Recognition** | OpenCV, dlib, face_recognition |
| **Authentication**   | Django Auth System             |
| **APIs**             | Django REST Framework (Optional for Live Data) |

---

# 🧑‍💻 Contributing
Contributions are always welcome! 💬

**1.Fork this repository**

**2.Create a new branch:**
```bash
git checkout -b feature/your-feature-name
```
**3.Commit your changes:**
```bash
git commit -m "Add your descriptive commit message"
```
**4.Push to your branch:**
```bash
git push origin feature/your-feature-name
```
**5.Create a Pull Request 🎉**


# 📜 License

This project is licensed under the MIT License — see the LICENSE
 file for details.



# ✨ Author

Avaneesh Pathak

📧 avaneeshpathak900@gmail.com

🔗 GitHub Profile



#
