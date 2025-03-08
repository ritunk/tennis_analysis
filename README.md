===============================
🎾 AI/ML Tennis Analysis System
===============================

This project analyzes **tennis players in a video** to measure **player speed, ball shot speed, and number of shots**. It uses **YOLOv8 for object detection** and **CNNs for keypoint detection**, making it an excellent hands-on project for **computer vision and deep learning**.

🚀 Features:
- **Detects and tracks players & tennis ball** in a video.
- **Calculates player movement speed & ball shot speed**.
- **Uses CNN-based court keypoint detection** for accurate tracking.
- **Generates an output video** with overlays for analysis.

===============================
📂 Project Structure
===============================
tennis_analysis/
├── models/                    # Trained models (Git LFS required)
│   ├── yolo5_last.pt          # Fine-tuned YOLO model (Download separately)
│   ├── yolov8x.pt             # YOLOv8 model (Download separately)
│   ├── keypoints_model.pth    # Court keypoint detection model
│
├── input_videos/              # Raw input tennis videos
│   ├── input_video.mp4
│
├── output_videos/             # Processed videos with tracking overlays
│
├── training/                  # Training scripts for models
│   ├── tennis_ball_detector_training.ipynb
│   ├── tennis_court_keypoints_training.ipynb
│
├── trackers/                  # Object tracking scripts
│   ├── ball_tracker.py
│   ├── player_tracker.py
│
├── main.py                    # Main script to run analysis
├── requirements.txt            # Required Python dependencies
├── .gitignore                  # Ignore unnecessary files
├── README.md                   # Project documentation

===============================
🛠️ Installation & Setup
===============================
1️⃣ Clone the Repository:
    git clone https://github.com/ritunk/tennis_analysis.git
    cd tennis_analysis

2️⃣ Install Dependencies:
    python -m venv venv
    source venv/bin/activate  # Mac/Linux
    venv\Scripts\activate     # Windows
    

===============================
🚀 Running the Project
===============================
1️⃣ Run the Main Script:
    python main.py

2️⃣ Check the Output Video:
Open:
    output_videos/output_video.mp4
This video will display **player & ball tracking overlays**.

===============================
📚 Training (Optional)
===============================
If you want to **train your own models**, use the Jupyter notebooks:
    jupyter notebook training/tennis_ball_detector_training.ipynb
    jupyter notebook training/tennis_court_keypoints_training.ipynb

===============================
👨‍💻 Technologies Used
===============================
- **Python** 🐍
- **YOLOv8 (Ultralytics)** 🚀
- **OpenCV** 📷
- **PyTorch** 🔥
- **Deep Learning (CNNs)** 🧠

===============================
💡 Contribution
===============================
Feel free to **fork this repository** and submit **pull requests**. Contributions are welcome! 🚀

===============================
🎾 Enjoy Analyzing Tennis Matches! 🚀
===============================

📌 `.gitignore`
===============================
# Ignore large files and unnecessary directories
*.pt
*.pth
*.mp4
*.avi
*.log
models/
runs/
output_videos/
venv/
__pycache__/

📌 `requirements
===============================
ultralytics
torch
torchvision
pandas
numpy
opencv-python
matplotlib
tqdm
