# Real-Time Pose Estimation

This project implements a real-time pose estimation system using Django for the backend and integrated web functionality for user interaction. The system detects and evaluates human poses from live webcam input or uploaded images. The project can be used for applications like fitness monitoring, activity recognition, and real-time pose correction.

## Features

- **User Authentication**: Secure user registration, login, and logout functionality.
- **Pose Detection**: Real-time pose detection using webcam input or image uploads.
- **Web Interface**: Interactive HTML pages for easy navigation.
- **Data Visualization**: Keypoint-based pose representation and analysis.
- **CSV-Based Pose Analysis**: Uses a dataset (`pose.csv`) for reference and testing pose classifications.

## Project Structure

### 1. Backend
The backend is powered by Django, which provides robust support for database handling and user management:
- **`posedetect/`**:
  - **`settings.py`**: Configurations for the Django application.
  - **`urls.py`**: URL routing for the application.
  - **`views.py`**: Handles business logic like pose detection, user authentication, and data processing.
  - **`models.py`**: Placeholder for database models.
- **Database**:
  - SQLite is used as the database for managing user accounts and session data.

### 2. Frontend
The user interface is designed with HTML, CSS, and JavaScript:
- **Templates**:
  - `camera.html`: Displays the live webcam feed for pose detection.
  - `login.html` and `signup.html`: Enable user authentication.
  - `about.html` and `image.html`: Provide additional application functionality.
- **Static Files**:
  - `script.js`: Handles dynamic interactions.
  - `style.css` and `webstyle.css`: Manage styling for the application.

### 3. Data
- **Pose Dataset (`pose.csv`)**:
  - Contains labeled keypoints representing various poses like pushups and squats.
  - Used for validation and pose analysis.

## Installation

### Prerequisites
Ensure the following are installed:
- Python 3.8 or above
- Django 4.2 or above
- Required Python packages (listed in `requirements.txt`)


## Usage

1. **Sign Up and Log In**:
   - Register and log in to access the features.
2. **Pose Detection**:
   - Navigate to the "Camera" page for real-time pose detection.
   - Alternatively, upload an image for static pose analysis.
3. **View Results**:
   - The application will display keypoints, detected poses, and additional analytics.

## Files of Interest

- **`views.py`**:
  - Implements pose detection and other backend logic.
- **`pose.csv`**:
  - Dataset used for pose analysis.
- **`camera.html`**:
  - User interface for real-time pose detection.

