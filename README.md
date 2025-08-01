# 📸 Smart Attendance System using Face Recognition

A Python-based attendance management system that leverages real-time **face recognition** for fast, automated, and reliable attendance marking using your system's webcam.

---

## ✨ Features

- 🔐 **Face Registration**: Add new user faces using webcam via `Add_faces.py`.
- 🤖 **Automated Attendance**: Recognize and log attendance automatically with timestamps.
- 🧾 **CSV Logging**: Saves attendance records in daily `.csv` files with date-based naming.
- 🖥️ **Simple CLI Usage**: Easy-to-run Python scripts — no complex setup required.

---

## 📁 Project Structure

| File/Folder               | Description                                           |
|--------------------------|-------------------------------------------------------|
| `app.py`                 | Main script to start the face recognition and log attendance |
| `Add_faces.py`           | Script to register new users via webcam              |
| `Attendance_*.csv`       | Generated CSVs that log daily attendance             |
| `Commands.txt`           | Notes or available commands for usage                |
| `.DS_Store`              | Mac system file (not relevant)                       |
| `README.md`              | You're reading it!                                   |
| `test.py` / `tempCodeRunnerFile.py` | Temporary/testing files for development        |

---

## 📦 Requirements

Install the following Python packages:

```bash
pip install opencv-python face-recognition numpy pandas
```
create a requirements.txt file:
opencv-python
face-recognition
numpy
pandas

Then install via:
```
pip install -r requirements.txt
```
🚀 Usage
1️⃣ Register New Faces
Run the following command to add user faces via webcam:
```
python Add_faces.py
```
2️⃣ Run the Attendance System
Once faces are registered, run the system:
```
python app.py
```
The webcam will open, recognize registered users, and automatically log their name and time in a CSV file like:
Attendance_01-08-2025.csv

📊 View Attendance Records
Open any Attendance_*.csv file to see who attended and when:
Name,Time for e.g. 
Rajat Sarkar,10:05:23


💡 Notes:
Make sure your webcam is accessible.

Avoid duplicate entries by registering each user only once.

CSVs are saved in the project directory by default.
