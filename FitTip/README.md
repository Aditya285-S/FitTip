# FitTip: Real-Time Posture Recognition and Correction

FitTip is an intelligent posture recognition and correction algorithm designed to help individuals perform exercises with proper form. By integrating **MediaPipe** for real-time body landmark detection and **TensorFlow** for analysis, FitTip provides actionable feedback to improve posture during workouts.

---

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Project Workflow](#project-workflow)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Example Demonstration](#example-demonstration)
8. [Contributing](#contributing)
9. [License](#license)

---

## Overview
As more people exercise at home or in the gym, ensuring proper posture is essential to prevent injuries and maximize performance. FitTip provides real-time feedback on body posture using advanced pose estimation techniques. It detects errors in common exercises like squats, planks, and push-ups and notifies the user with accuracy feedback.

---

## Features
- **Real-Time Pose Estimation**: Capture body landmarks using MediaPipe's Pose Detection.
- **Angle Analysis**: Calculate joint angles (e.g., elbows, knees) to determine posture correctness.
- **Error Detection**: Identify deviations from the correct posture and notify the user.
- **Accuracy Feedback**: Provide actionable feedback with accuracy scores.
- **User-Friendly Workflow**: Simple pipeline for posture analysis and correction.

---

## Technologies Used
- **Python**: Main programming language.
- **MediaPipe**: Pose Detection for identifying body landmarks.
- **TensorFlow**: Analysis and feedback model.
- **OpenCV**: Image processing for video feed.
- **Matplotlib**: Visualizations for demonstration.

---

## Project Workflow
The workflow of FitTip can be summarized as follows:

1. **Capture Frame**: Read video feed or images from a normal camera.
2. **Convert to RGB**: Preprocess the input to standard RGB format for MediaPipe.
3. **Pose Detection**: Extract body landmarks (joints like elbows, knees, wrists, etc.) using MediaPipe.
4. **Angle Calculation**: Measure joint angles and body inclination.
5. **Posture Analysis**:
   - Check if angles meet the thresholds for correct posture.
   - Notify users about accuracy.
6. **Feedback**: Provide results for pass/fail and corrective measures.

---

## Installation
Follow these steps to set up the project:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/FitTip.git
   cd FitTip
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the main script:
   ```bash
   python main.py
   ```

---

## Usage
To use FitTip:
1. Ensure your camera is connected.
2. Run the script to start posture detection.
3. Perform exercises like **squats** or **planks** in front of the camera.
4. FitTip will:
   - Detect your body landmarks.
   - Analyze angles and inclination.
   - Notify you if your posture is incorrect.

---

## Example Demonstration
### Squat Example
- **Correct Angle**: Knee joint angle between **90°-100°**.
- **Landmarks Used**: Hips, knees, and ankles.
- **Notification**: If knee angle <90° or >100°, feedback is provided.

Example Output:
```
Posture: Incorrect
Accuracy: 85%
Correction: Lower your hips to align with your knees.
```

---

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Create a Pull Request.

---
