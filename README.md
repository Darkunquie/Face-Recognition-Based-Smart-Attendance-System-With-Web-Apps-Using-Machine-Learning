# Attendance Management System with Facial Recognition

This project implements an Attendance Management System using facial recognition technology. The application is built using Python and leverages libraries such as OpenCV, Streamlit, and scikit-learn. It captures real-time video to recognize faces, records attendance, and displays the data interactively.

## Features

- **Real-time Face Detection**: Uses OpenCV's Haar Cascade Classifier to detect faces in real time.
- **Attendance Recording**: Records the attendance of recognized individuals and saves it to a CSV file.
- **Data Visualization**: Displays attendance data using Streamlit, with automatic refreshing.
- **Voice Feedback**: Provides voice feedback when attendance is taken using the SAPI.SpVoice library.

## Requirements

To run this project, you need the following libraries:

- OpenCV
- pandas
- Streamlit
- scikit-learn
- numpy
- pywin32 (for voice feedback)
- streamlit-autorefresh

You can install the required libraries using pip:

bash
#pip install opencv-python pandas streamlit scikit-learn numpy pywin32 streamlit-autorefresh

## Download Haar Cascade File:
Ensure you have the haarcascade_frontalface_default.xml file in the data directory. You can download it from the OpenCV GitHub repository.

## Create Attendance Directory:
Create a directory named Attendance in the root of the project to store attendance CSV files.

## Run the Face Capture Script:
Execute the face capture script to register faces:

Copy
python face_capture.py
Follow the prompts to enter your name and capture your face.

Train the Model:
After capturing faces, run the training script to build the KNN model:

Copy
python train_model.py
Start the Streamlit App:
Run the Streamlit app to visualize attendance:

Copy
streamlit run attendance_app.py
Usage
Face Capture: Run the face capture script to register new faces.
Attendance: Once the model is trained, run the attendance script. Press 'o' to mark attendance and 'q' to quit.
View Attendance: Access the Streamlit app to view the attendance data.
Notes
Ensure your camera is working and accessible.
Adjust the paths in the scripts as necessary based on your project structure.
The attendance records are saved in CSV format in the Attendance directory.


Feel free to modify any sections to better fit your project or personal style!
