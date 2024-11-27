# Plant-Disease-Detection_

🌿 Plant Disease Detection
This project is a machine learning-based web application that helps detect plant diseases by analyzing images of leaves. The app uses a trained deep learning model to identify diseases and their severity with high accuracy. It is built with TensorFlow, Keras, and Streamlit.

🎯 Features
Plant Disease Detection: Detects diseases in plant leaves with a high level of accuracy.
Real-time Predictions: Upload an image of a leaf, and the model will classify it as either healthy or diseased.
Wide Plant Support: The app supports 14 plant species and identifies 38 classes, including 26 diseases.
User-Friendly Interface: Simple and intuitive design powered by Streamlit.
🏗️ Technologies Used
Frameworks:
Streamlit for the web application.
TensorFlow/Keras for deep learning.
Languages: Python
Libraries:
TensorFlow/Keras for model training and prediction.
NumPy and PIL for image processing.
h5py for model loading.
🖼️ Dataset
The dataset used in this project is a collection of leaf images for various plants.
Key Stats:
Plant Species: 14 (e.g., Tomato, Grape, Apple, etc.)
Diseases: 26 unique diseases.
Total Classes: 38 (includes healthy images).
Dataset includes augmented images for robustness and better generalization.
🛠️ Setup Instructions
Prerequisites
Python 3.8 or higher.
Required Python libraries listed in requirements.txt.
Steps to Set Up
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/plant-disease-detection.git
cd plant-disease-detection
Create and activate a virtual environment:
bash
Copy code
python -m venv venv
source venv/bin/activate  # For macOS/Linux
venv\Scripts\activate     # For Windows
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Run the Streamlit app:
bash
Copy code
streamlit run main.py
🌟 Usage Instructions
Upload an Image: Choose a clear image of the affected plant leaf.
Analyze Results:
View the plant species and the detected disease (if any).
Check the confidence score for the prediction.
Review Recommendations: Follow the diagnosis for potential treatment.
📂 Project Structure
bash
Copy code
Plant Disease Detection/
│
├── main.py              # Main application file (Streamlit app)
├── bestmodel1.h5        # Trained model for plant disease detection
├── requirements.txt     # List of dependencies
├── README.md            # Project documentation
├── dataset/             # Optional: Directory for dataset
│   ├── train/           # Training data
│   └── test/            # Testing data
📊 Supported Plants and Diseases
Supported Plants:

Tomato, Grape, Orange, Soybean, Squash, Potato, Corn, Strawberry, Peach, Apple, Blueberry, Cherry, Pepper, Raspberry.
Common Diseases Detected:

Tomato Late Blight, Powdery Mildew, Apple Scab, Tomato Yellow Leaf Curl Virus, Black Rot, etc.
🤖 Model Details
Architecture: The model is a convolutional neural network (CNN) trained using TensorFlow/Keras.
Input Size: 128x128 RGB images.
Output: Softmax probabilities for 38 classes (plant + disease).
Training: The model was trained on augmented images to improve generalization.
