Emotion-Based Music Recommendation System
A simple yet powerful application that recommends music on YouTube based on your real-time facial expressions. This project leverages computer vision and deep learning to detect your emotion and curate a playlist that matches your mood, optionally filtered by your favorite artist.

🌟 Features
Real-Time Emotion Detection: Uses your webcam to detect emotions like Happy, Sad, Angry, Neutral, and Surprise in real-time.

YouTube Music Recommendations: Get a list of songs, playable on YouTube, that match your current mood.

Artist-Based Filtering: Enter the name of an artist to get recommendations specifically from them.

Simple Web Interface: An easy-to-use and interactive interface built with Streamlit to display the camera feed, detected emotion, and song suggestions.

Extensible: Easy to integrate with other music APIs.

⚙️ How It Works
The application follows a simple workflow:

Artist Input (Optional): The user can enter the name of an artist to tailor the music recommendations.

Capture Video: The system accesses the webcam to capture a live video stream.

Detect Faces: It uses a Haar Cascade classifier from OpenCV to detect faces in each frame.

Recognize Emotion: The detected face is passed to a pre-trained Convolutional Neural Network (CNN) model which classifies the emotion.

Recommend Music: Based on the predicted emotion and the optional artist name, the application uses the YouTube API to fetch and suggest relevant songs.

Display: The video feed, detected emotion, and music recommendations are displayed on the Streamlit web interface.

🚀 Getting Started
Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites
Make sure you have Python 3.8 or higher installed on your system. You will also need pip to install the required libraries. You'll also need a YouTube Data API key.

Installation
Clone the repository:

git clone [https://github.com/your-username/Emotion-Based-Music-Recommendation-System.git](https://github.com/your-username/Emotion-Based-Music-Recommendation-System.git)
cd Emotion-Based-Music-Recommendation-System

Create a virtual environment (recommended):

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install the dependencies:

pip install -r requirements.txt

(You will need to create a requirements.txt file containing libraries like streamlit, opencv-python, tensorflow, numpy, and google-api-python-client.)

Download Pre-trained Models:

You will need a pre-trained model for emotion detection. Place it in a models directory.

You will also need the Haar Cascade file (haarcascade_frontalface_default.xml) for face detection.

Running the Application
Start the Streamlit app:

streamlit run app.py

Open your browser:
Navigate to the local URL provided by Streamlit (usually http://localhost:8501) to see the application in action.

Allow Webcam Access:
Your browser will prompt for permission to use your webcam. Click "Allow".

Usage
Once the application is running, you can optionally enter an artist's name in the input field. Then, position your face in front of the camera. The system will draw a box around your face, detect your emotion, and display a list of recommended YouTube songs on the screen.

📸 Screenshot
(Add a screenshot of your application here to give users a visual idea of your project)

💡 Future Improvements
[ ] Integrate with the Spotify API for dynamic playlist generation.

[ ] Improve the accuracy of the emotion detection model by training it on a larger dataset.

[ ] Allow users to create profiles and save their music preferences.

[ ] Deploy the application to a cloud service like Heroku or AWS.

🤝 Contributing
Contributions are welcome! If you have ideas for new features or improvements, please create an issue or submit a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
