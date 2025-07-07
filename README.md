# SmartAttendance
Face Recognition Attendance System
SmartAttendance – Face Recognition Attendance System
SmartAttendance is a real-time facial recognition attendance tracking system developed using Python, OpenCV, and the face_recognition library. It detects and identifies known faces from webcam input and automatically logs attendance into a CSV file with the person's name, current time, and date.

🔧 Features
Real-time face detection via webcam

Face recognition from pre-saved images

Marks attendance only once per person per day

Saves attendance logs in CSV format

Lightweight, fast, and easy to set up

🖼️ How It Works
You store known face images in a folder (with filenames as names of the people).

The webcam captures live frames and matches detected faces with the stored ones.

If a face matches and has not been marked present for the day, it logs the name, time, and date in a CSV file.

You can review attendance records in the generated file: attendance.csv

📁 Directory Structure
javascript
C:/SmartAttendance/
├── known_faces/
│   ├── Alice.jpg
│   ├── Bob.jpg
├── attendance.csv
├── attendance_script.py
known_faces/: contains all reference face images (filenames are treated as names)

attendance.csv: stores daily attendance logs

attendance_script.py: the main script file

▶️ How to Run
Install required packages:

pip install opencv-python face_recognition numpy
Place reference face images inside the known_faces/ folder.

Run the script:

python attendance_script.py
A webcam window will open. Detected known faces will be labeled and logged.

Press Q to quit.

✅ Requirements
Python 3.6+

OpenCV

face_recognition

dlib (automatically installed with face_recognition)

A working webcam

📋 Output Example
Example attendance.csv:

name,time,date
ALICE,09:12:45,2025-07-07
BOB,09:15:23,2025-07-07

📄 License
This project is open source and free to use.
