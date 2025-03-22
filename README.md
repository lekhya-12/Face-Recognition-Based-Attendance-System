## Face Recognition based Attendance Management System (FaceIT)
Face Recognition based Attendance Management System with a Flask web application.

### Table of Contents
- [Features](#features)
- [Installation and Usage](#installation-and-usage)
- [Technologies Used](#technologies-used)
- [Methodology](#methodology)

### Features
- Face detection and recognition
- Attendance management
- Generates attendance reports and can download as excel files
- Secure teacher and student login
- Interactive user interface
- Can detect multiple faces and mark attendance at a time 
- Works in bright and low light conditions

### Installation and Usage
1. Clone the repository
2. Install the required dependencies:
    ```
    pip install -r requirements.txt
    ```
3. Replace the training images with your own set of images in the folder `Training images`.
4. Open the `app.py` file and change the file paths as per your system.
5. Run the `app.py` file.

### Technologies Used
- **Programming Languages:** Python
- **Libraries:** OpenCV, dlib, face-recognition
- **Database:** SQLite
- **Web Application:** Flask, HTML, CSS, JavaScript

### Methodology
- **Environment Setup:** Created a conda environment and installed necessary dependencies including OpenCV, dlib, face-recognition, and Flask.
- **Face Detection:** Converted images to black and white, then used HOG to detect faces by comparing image gradients.
- **Face Embedding:** Used 128-dimensional vectors and the triplet loss function for distinguishing between faces.
- **Face Recognition:** Utilized Euclidean distance with a threshold of 0.5 to compare the generated face encodings with the actual encodings of the training images to recognize the faces.
- **Database Connection:** Stored attendance data in a SQLite database.
- **Web Application:** Developed a Flask-based web app for real-time attendance capturing and management.
