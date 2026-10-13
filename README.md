# Face Recognition Attendance System

A Python-based attendance management system that uses facial recognition to identify registered people and automatically record their attendance with timestamps in a CSV file.

## Features

- Real-time face detection using a webcam
- Face recognition using the `face_recognition` library
- Automatic attendance recording
- Date-independent time tracking in `HH:MM:SS` format
- Duplicate attendance prevention during the same attendance file session
- CSV-based attendance storage
- Visual display of recognized and unknown faces

## Technologies Used

- Python
- OpenCV
- NumPy
- face_recognition
- CSV for attendance storage

## Project Structure

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

Note: The image folder name in the code must match the actual folder name. The current code uses `Images`.

## Prerequisites

- Python installed on your computer
- A working webcam
- Git (optional, for version control)
- Visual Studio Code or another Python editor

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Arya-gunji/Face-Recognition-Attendance-System.git
   ```

2. Open the project directory:

   ```bash
   cd Face-Recognition-Attendance-System
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

1. Place the registered person's images inside the `Images` folder.
2. Use clear images containing one visible face per file.
3. Ensure `Attendance.csv` exists and contains this header:

   ```csv
   Name,Time
   ```

4. Make sure your webcam is connected and accessible.

## Run the Project

Execute the following command:

```bash
python attendance.py
```

The webcam opens and attempts to recognize registered faces. Recognized names are displayed on the video, and attendance is recorded in `Attendance.csv`.

Press **Q** to close the webcam window.

## Output

The attendance file contains records in the following format:

```csv
Name,Time
ARYA,19:49:30
RAHUL,11:59:03
```

The example records are illustrative. Actual timestamps depend on when attendance is recorded.

## Troubleshooting

- **Camera not opening:** Check camera permissions and ensure another application is not using the webcam.
- **Module not found:** Install the dependencies using `pip install -r requirements.txt`.
- **Face not recognized:** Use clear, well-lit images and verify that the person's image exists in the `Images` folder.
- **Face recognition installation error:** The `face_recognition` library depends on `dlib`, which may require additional setup, especially on Windows.

## Privacy and Security

This project processes facial images, which are sensitive biometric data. Use it only with appropriate consent. Store images and attendance records securely, and avoid publishing real personal images or attendance information in a public repository.

## Future Enhancements

- Store attendance with date and time
- Add a database for attendance records
- Build a graphical user interface
- Generate daily and monthly attendance reports
- Add authentication and access controls

## Author

**Arya Gunji**

GitHub: [Arya-gunji](https://github.com/Arya-gunji)

---

If you find this project useful, consider starring the repository.
