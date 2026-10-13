
# Face Recognition Attendance System

A Python-based Face Recognition Attendance System that automatically identifies registered faces using a webcam and records attendance with timestamps in a CSV file.

## 🔗 Project Links

- **GitHub Repository:** https://github.com/Arya-gunji/Face-Recognition-Attendance-System
- **Python Source Code:** https://github.com/Arya-gunji/Face-Recognition-Attendance-System/blob/main/attendance.py
- **README:** https://github.com/Arya-gunji/Face-Recognition-Attendance-System/blob/main/README.md
- **Author GitHub Profile:** https://github.com/Arya-gunji
- **LinkedIn:** https://www.linkedin.com/in/arya-gunji/

## 🚀 Features

- Real-time face detection using a webcam
- Face recognition using the `face_recognition` library
- Automatic attendance marking
- Attendance timestamps
- CSV-based attendance storage
- Duplicate attendance prevention within the same attendance file
- Visual identification of recognized and unknown faces

## 🛠️ Technologies Used

- Python
- OpenCV
- NumPy
- face_recognition
- CSV

## 📁 Project Structure

```text
Face-Recognition-Attendance-System/
├── Images/
│   ├── Arya.jpg
│   └── Rahul.jpeg
├── attendance.py
├── Attendance.csv
├── Project Structure
├── README.md
└── requirements.txt
```

**Note:** The current Python code uses `Images` as the folder name. Make sure the actual folder name matches, including capitalization.

## 💻 Requirements

- Python 3.10 or another version compatible with the required libraries
- Webcam
- pip package installer
- Windows, Linux, or macOS
- VS Code or another Python editor (optional)

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Arya-gunji/Face-Recognition-Attendance-System.git
```

### 2. Navigate to the Project Folder

```bash
cd Face-Recognition-Attendance-System
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If installation of `face_recognition` fails on Windows, additional setup for `dlib` may be required.

## ⚙️ Configuration

1. Add registered people's images to the `Images` folder.
2. Use clear images with one face per image.
3. Ensure `Attendance.csv` exists.
4. Add the following header to the CSV file:

```csv
Name,Time
```

5. Connect your webcam and allow camera access.

## ▶️ How to Run

Run this command from the project directory:

```bash
python attendance.py
```

The application opens the webcam and attempts to recognize faces.

- Recognized faces are displayed with their names.
- Unknown faces are displayed as `UNKNOWN`.
- Recognized attendance is recorded in `Attendance.csv`.
- Press **Q** to close the webcam window.

## 📊 Sample Output

The CSV attendance file follows this format:

```csv
Name,Time
ARYA,19:49:30
RAHUL,11:59:03
```

These are sample records, not live output.

## 🔍 Troubleshooting

**Camera not opening**
- Check camera permissions.
- Close other applications that may be using the webcam.

**Module not found**
- Run `pip install -r requirements.txt`.
- Confirm that you are using the correct Python environment.

**Face not recognized**
- Use clear, well-lit images.
- Confirm that the image files are in the correct folder.

**face_recognition installation error**
- Check the compatibility of Python and `dlib`.
- Follow the installation instructions for your operating system.

## 🔐 Privacy and Security

Facial images are sensitive biometric information. Obtain appropriate consent before collecting or processing images. Do not upload private facial images or real attendance records to a public repository without permission.

## 🔮 Future Enhancements

- Record both date and time
- Store attendance in MySQL
- Generate daily and monthly attendance reports
- Add a graphical user interface
- Implement authentication and role-based access

## 👨‍💻 Author

**Arya Gunji**

- GitHub: https://github.com/Arya-gunji
- LinkedIn: https://www.linkedin.com/in/arya-gunji/

---

⭐ If you find this project useful, consider starring the repository.
