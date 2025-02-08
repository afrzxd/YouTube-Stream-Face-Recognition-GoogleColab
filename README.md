# YouTube-Stream-Face-Recognition-GoogleColab
This project is a real-time face recognition system that processes live streaming videos from YouTube. It detects and recognizes faces using MTCNN for face detection and DeepFace for face verification. The recognized faces are compared against a set of reference images to identify known individuals.

# YouTube Stream Face Recognition System

A Python-based facial recognition system that can detect and identify faces from YouTube streams/videos using MTCNN and DeepFace.

## 🌟 Features

- Real-time face detection using MTCNN (Multi-Task Cascaded Convolutional Networks)
- Face recognition and verification using DeepFace with VGG-Face model
- Support for YouTube video/stream processing
- Image enhancement with contrast adjustment
- Automatic face capture and storage
- Frame-by-frame analysis and storage
- Visual output with confidence scores
- Reference image comparison system

## 📋 Prerequisites

```bash
- Python 3.x
- OpenCV (cv2)
- NumPy
- yt-dlp
- DeepFace
- MTCNN
- Matplotlib
- IPython (for Colab compatibility)
```

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/afrzxd/YouTube-Stream-Face-Recognition-GoogleColab.git
cd YouTube-Stream-Face-Recognition-GoogleColab
```

2. Install required packages:
```bash
pip install opencv-python numpy yt-dlp deepface mtcnn matplotlib ipython
```

## 📝 Usage

1. Place reference images in the root directory with the format: `NUMBER_Name.jpg`

2. Update the YouTube URL in the code:
```python
url = "YOUR_YOUTUBE_URL"
```

3. Run the script:
```python
python main.py
```

## 🎯 How It Works

1. The system loads reference images from the directory
2. Connects to the specified YouTube stream/video
3. Processes frames using MTCNN for face detection
4. Applies image enhancement for better detection
5. Compares detected faces with reference images using DeepFace
6. Stores detected faces and processed frames
7. Displays results with confidence scores

## 📂 Output Structure

- `/data` - Contains captured face images
- `/frames` - Contains processed video frames

## ⚙️ Configuration Options

- `max_duration`: Set maximum processing time (default: 40 seconds)
- `capture_count`: Set number of captures to store
- Face detection confidence threshold: 0.9
- Face recognition similarity threshold: 50%

## 🔍 Features Details

- **Enhanced Face Detection**: Uses MTCNN with optimized parameters
- **Image Enhancement**: Implements CLAHE (Contrast Limited Adaptive Histogram Equalization)
- **Expanded Face Area**: Includes additional area for better recognition with accessories
- **Real-time Visualization**: Shows detection results with bounding boxes and confidence scores

## 📊 Output Visualization

- Real-time frame display with detected faces
- Summary display of captured faces
- Frame sequence visualization

## ⚠️ Limitations

- Requires stable internet connection for YouTube streaming
- Performance depends on video quality and lighting conditions
- May have varying accuracy with different face angles and expressions

## 🤝 Contributing

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

