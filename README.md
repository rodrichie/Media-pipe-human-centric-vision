# MediaPipe Human-Centric Vision Tasks Demo

This notebook demonstrates various human-centric vision tasks using the MediaPipe library. It includes tasks such as face detection, face mesh, pose detection, and 3D head pose estimation. The notebook also provides utilities for processing video frames, detecting faces, and calculating yaw, pitch, and roll angles.

## Table of Contents

1. [Setup and Imports](#setup-and-imports)
2. [Loading Video Frames](#loading-video-frames)
3. [Face Detection](#face-detection)
4. [Face Mesh](#face-mesh)
5. [Pose Detection](#pose-detection)
6. [3D Head Pose Estimation](#3d-head-pose-estimation)
7. [Video Processing](#video-processing)
8. [Utilities](#utilities)

## Setup and Imports

The notebook begins by installing the necessary libraries and importing required modules. The main libraries used are:

- `mediapipe`: For human-centric vision tasks.
- `cv2`: For video processing.
- `numpy`: For numerical operations.
- `matplotlib`: For displaying images.
- `pathlib`: For handling file paths.

## Loading Video Frames

The notebook provides a function `load_video_frame` to load a specific frame from a video file. This function uses OpenCV to read the video and extract the desired frame.

## Face Detection

The `detect_faces` function uses MediaPipe's face detection model to detect faces in an image. It returns the detected faces and an annotated image with the detections drawn.

## Face Mesh

The `get_face_mesh` function uses MediaPipe's face mesh model to generate a detailed face mesh. It returns the face landmarks and an annotated image with the mesh drawn.

## Pose Detection

The `detect_pose` function uses MediaPipe's pose detection model to detect body poses in an image. It returns the pose landmarks and an annotated image with the landmarks drawn.

## 3D Head Pose Estimation

The notebook includes functions for 3D head pose estimation using OpenCV and MediaPipe. The `calculate_yaw_pitch_roll` function calculates the yaw, pitch, and roll angles of the face. The `detect_faces_with_3d_pose` function detects faces and calculates their 3D head pose.

## Video Processing

The notebook provides functions for processing videos, including trimming videos based on face detection and splitting videos into sliding windows. The `trim_videos` function trims input videos based on face detection, while the `split_into_windows` function splits the trimmed video into sliding windows.

## Utilities

The notebook includes several utility functions for displaying results, calculating coordinates, and writing trimmed videos. The `display_results` function displays the original and processed images side by side. The `get_face_mesh_coords` function converts face mesh landmarks to image coordinates.

## Usage

To use this notebook, ensure you have the required libraries installed. You can install them using pip:

```bash
pip install mediapipe opencv-python numpy matplotlib
```

Then, run the notebook cells sequentially to perform the desired tasks. You can modify the video paths and parameters as needed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- MediaPipe: [https://mediapipe.dev/](https://mediapipe.dev/)
- OpenCV: [https://opencv.org/](https://opencv.org/)
- NumPy: [https://numpy.org/](https://numpy.org/)
- Matplotlib: [https://matplotlib.org/](https://matplotlib.org/)
```

This `README.md` provides an overview of the notebook's contents, setup instructions, and usage guidelines. You can customize it further based on your specific needs.
