# Tennis Ball Detection using YOLOv5 and Streamlit

This project demonstrates real-time tennis ball and player detection from video input using a custom-trained YOLOv5 model. The application is built with Streamlit for an interactive user interface.

**[Live Application](https://tennisballandperson.streamlit.app)**

## Features

- Upload video files for processing
- Displays the progress of object detection
- Shows output video with tennis ball and player detection after processing

## Setup Instructions

### 1. Clone the Repository

```bash
git clone <repository-url>
cd yolov5
```

### 2. Install Dependencies

Make sure you have Python installed. Then, install the required libraries:

```bash
pip install -r requirements.txt
```

### 3. Model Setup

Place the custom-trained YOLOv5 model file in the `yolov5/runs/exp/weights/best.pt`.

### 4. Run the Application Locally

Run the following command in the `yolov5` directory:

```bash
streamlit run app.py
```

## File Structure

```
yolov5/
├── app.py                  # Streamlit application file
├── runs/
│   └── exp/
│       └── weights/
│           └── best.pt     # Trained YOLOv5 model weights
└── data/                   # Contains video input files
```

## Usage

1. Launch the Streamlit application.
2. Upload a video file in `.mp4` format.
3. Wait for the detection to process; the completion percentage will be displayed.
4. After processing, view the output video with detections highlighted.

## Example

Upload a sample tennis match video to detect player movements and tennis ball positions, using real-time updates for progress.

## Dependencies

- Streamlit
- PyTorch
- OpenCV
- YOLOv5