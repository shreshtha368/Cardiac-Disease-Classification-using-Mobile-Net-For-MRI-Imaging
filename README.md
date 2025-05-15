Cardiac Disease Classification using MobileNet for MRI Imaging
📌 Overview
This project focuses on automating the classification of cardiac MRI scans into normal and abnormal categories using a deep learning model based on the MobileNet architecture. The goal is to assist in early diagnosis and improve the efficiency of cardiac disease detection.

🧠 Model Architecture
Base Model: MobileNet (lightweight CNN for feature extraction)

Modifications:

Added global average pooling and a dense output layer (sigmoid activation)

Used dropout regularization to avoid overfitting

Loss Function: Binary Cross-Entropy

Optimizer: Adam with an initial learning rate of 1e-4

Evaluation Metrics: Accuracy, Precision, Recall, F1-Score

📊 Dataset
Source: CAD Cardiac MRI Dataset

Total Images: 63,425

Classes: Normal and Abnormal

Image Size: Resized to 128x128 pixels

Normalization: Pixel values scaled to [0, 1]

🧪 Data Augmentation
To improve generalization with limited data:

Random rotations (±15°)

Horizontal/vertical translations (up to 10%)

Zoom and shear transformations

Horizontal flipping

📈 Results
Class	Precision	Recall	F1-Score
Normal	0.86	0.84	0.85
Abnormal	0.78	0.81	0.79
Overall	0.83	0.83	0.83

Validation Accuracy: 78.37%

Final Training Accuracy: 76.80%

Overall Accuracy: 83%

📌 Key Highlights
Achieved robust classification on cardiac MRI data using MobileNet

Reduced overfitting through strategic data augmentation and dropout

Demonstrated potential for real-world clinical deployment

🖼️ Sample Output

Sample predictions showing model accuracy in distinguishing cardiac structures.

🛠️ Tools & Libraries
Python

TensorFlow / Keras

NumPy, Matplotlib, OpenCV

Scikit-learn

🚀 How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/Cardiac-MRI-MobileNet.git
cd Cardiac-MRI-MobileNet
Install requirements:

bash
Copy
Edit
pip install -r requirements.txt
Run the notebook:

bash
Copy
Edit
jupyter notebook 21BAI1178_DL_Cardio_MRI_Classification.ipynb
🧾 Citation
If you use this work, please cite the corresponding paper:

cpp
Copy
Edit
Shreshtha Nagpal, Thomas Abraham, “Cardiac Disease Classification using Mobile-Net For MRI Imaging”, Vellore Institute of Technology, Chennai, 2024.
