Real-Time Face Recognition Using FaceNet on TensorFlow 2.X
A robust, real-time facial recognition system built using the pre-trained FaceNet model and MTCNN for face detection.


📌 Features
Real-time face detection and recognition

Supports multiple faces in a single frame

Easily add new users to the system

Uses FaceNet for facial embeddings

Built with TensorFlow 2.X

Pre-trained weights available for quick start

🚀 Quick Start
# Clone the repository
git clone https://github.com/yourusername/Face-recognition-Using-Facenet-On-Tensorflow-2.X.git
cd Face-recognition-Using-Facenet-On-Tensorflow-2.X

# Install dependencies
pip install -r requirements.txt

# Download pretrained weights and place in the root directory
# Add face images
mkdir Faces/YourName
# Add 2-3 clear face images into this directory

# Train the model
python train_v2.py

# Start real-time recognition
python detect.py

📘 Detailed Usage
🏋️ Training
Use 2–3 clear and well-lit face images per person

Images should be from slightly different angles

Encodings will be saved to encodings/encodings.pkl

👁️ Real-time Detection
Press q to quit

Shows confidence scores for detected faces

Unknown faces will be labeled as "Unknown"

🗂️ Project Structure
graphql
Copy
Edit
Face-recognition-Using-Facenet-On-Tensorflow-2.X/
├── architecture.py               # FaceNet model architecture (TF 2.X)
├── detect.py                     # Real-time detection script
├── train_v2.py                   # Face encoding training script
├── Custo_face_net_1.ipynb        # Notebook for custom model testing
├── facenet_keras_weights.h5      # Pre-trained FaceNet weights
├── encodings/
│   └── encodings.pkl             # Generated facial embeddings
├── Faces/                        # Folder for face images
│   ├── Person1/
│   └── Person2/
├── MEDIA/
│   └── gif.gif                   # Demo animation
├── LICENSE
└── README.md
🧰 Dependencies
TensorFlow >= 2.3.0

NumPy

OpenCV-Python

MTCNN

Scikit-learn

SciPy

Install with:

bash
Copy
Edit
pip install -r requirements.txt
🛠️ Troubleshooting
Shape mismatch? — Ensure you're using the correct facenet_keras_weights.h5 file

Slow performance? — Reduce camera resolution in detect.py

Poor accuracy? — Make sure face images are well-lit, front-facing, and not blurry

🧠 Credits
FaceNet Paper: FaceNet: A Unified Embedding for Face Recognition and Clustering

Inspired by Practical-AI/Face

Based on: Face Recognition with FaceNet and MTCNN

Let me know if you want to add sections for model architecture details or Docker setup!
