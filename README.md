# Driver Monitoring System (DMS)

The Driver Monitoring System (DMS) is designed to enhance road safety by detecting driver drowsiness and distractions in real-time. Utilizing computer vision and deep learning techniques, the system monitors the driver's facial features and actions to identify signs of fatigue or unsafe behaviors.

## Objectives

- Detect driver drowsiness and alertness.
- Identify actions such as yawning and phone usage.
- Provide real-time alerts to prevent accidents.

## Key Components

1. **Video Capture**: Uses a camera to capture live video of the driver.
2. **Facial Detection and Tracking**: Employs Mediapipe for facial landmark detection.
3. **Feature Extraction**: Analyzes eye and mouth landmarks to compute aspect ratios.
4. **Action Detection**: Utilizes pre-trained CNN models to detect specific driver actions.
5. **Alert Mechanism**: Generates audible alerts for detected drowsiness or distractions.

## Technologies Used

- **OpenCV**: For video capture and processing.
- **Mediapipe**: For facial detection and tracking.
- **TensorFlow**: For deep learning model implementation.
- **Pygame**: For generating alert sounds.

## 🔧 Requirements

### Libraries
    
    ```bash
    opencv-python==4.7.0.72
    mediapipe==0.9.1.0
    pygame==2.1.2
    numpy==1.23.5
    scipy==1.10.0
    tensorflow==2.11.0  # or use PyTorch if applicable
    dlib==19.24.0
    imutils==0.5.4
    ```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Affan-04/driver-monitoring-system.git
   cd driver-monitoring-system
   ```

2. Install the dependencies using:

    ```bash
    pip install -r requirements.txt
    ```

3. Create a Virtual Environment
    ```bash
    python -m venv venv
    Windows: venv\Scripts\activate
    ```

4. Run the project
    ```bash
    python dms.py --checkpoint models/model_split.h5 --webcam 0
    ```



<p align="center">
  <img src="img\image_url_1.gif" width="200", height="200"/>
  <img src="img\image_url_2.gif" width="200", height="200"/>
</p>


