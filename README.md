# Face Attendance System Using Python and OpenCV

## Project Overview
The **Face Attendance System** is an automated attendance management system that uses **face recognition** to mark attendance in real-time. It eliminates manual attendance sheets, making tracking **faster, more accurate, and efficient**. The system captures faces, trains a recognition model, and automatically updates attendance in a **daily CSV file**.

---

## Features

### 1. Face Registration
- Capture multiple images of a person’s face using a webcam.  
- Assigns each person a **unique ID**.  
- Stores images in a **dataset** folder for training.

### 2. Train Face Recognition Model
- Uses **LBPH (Local Binary Patterns Histograms)** algorithm from OpenCV.  
- Trains the model on captured face images.  
- Saves the trained model for future attendance marking.

### 3. Automated Attendance Marking
- Detects and recognizes faces **in real-time**.  
- Marks attendance in a **daily CSV file**.  
- Prevents duplicate attendance marking for the same student.

### 4. Daily Attendance Records
- Generates a **new CSV file every day**.  
- Marks students as **"Present"** or **"Absent"**.

---
Face-Attendance-System/
│
├─ dataset/ # Captured face images for training
├─ trainer/ # Stores the trained LBPH face recognition model
├─ name_id_map.csv # Maps student names to unique IDs
├─ attendance_YYYY-MM-DD.csv # Daily attendance CSV file
├─ face_attendance.py # Main Python script for the system


---

## Technology Stack
- **Python** – Core programming language  
- **OpenCV** – Face detection and recognition  
- **Pillow (PIL)** – Image processing  
- **NumPy** – Handling image arrays  
- **CSV** – Attendance record management  
- **Haar Cascade Classifier** – Detect faces in images and video streams  

---

## How It Works

1. **Register Faces**  
   Users input their name, and the system captures 50 images of their face using a webcam. Images are stored in the **dataset/** folder for training.

2. **Train Model**  
   Captured images are used to train the **LBPH face recognizer**. The trained model is saved in `trainer/trainer.yml`.

3. **Take Attendance**  
   The system detects and recognizes faces in real-time. Attendance is updated automatically in a daily CSV file. Students are marked as "Present" or "Absent," and duplicate markings are prevented.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Face-Attendance-System.git
cd Face-Attendance-System
Usage

Register Face → Capture images of a new student.

Train Model → Train the recognition model with the captured dataset.

Take Attendance → Start real-time attendance marking using the webcam.

Exit → Close the system.

Key Highlights

Fully automated face recognition attendance system.

Generates daily attendance CSV files with "Present/Absent" status.

Easy to extend for schools, colleges, or offices.

Uses OpenCV’s robust LBPH face recognition algorithm.

## Directory Structure

