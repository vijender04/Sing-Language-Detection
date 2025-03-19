# Sign Language Detection Project

This project is a real-time sign language detection system that uses a deep learning model to recognize hand gestures corresponding to the letters of the alphabet (A-Z). The system captures video input from a webcam, processes the hand landmarks using MediaPipe, and predicts the corresponding letter using a pre-trained TensorFlow model. The detected letters can be combined to form words, which are then spoken aloud using a text-to-speech engine.

## Features

- **Real-time Hand Gesture Recognition**: Detects hand gestures corresponding to the letters A-Z.
- **Text-to-Speech**: Converts the detected letters into spoken words.
- **Interactive Interface**: Allows users to manually store letters to form words.
- **Bounding Box and Landmarks Visualization**: Displays the hand landmarks and bounding box on the video feed.

## Requirements

To run this project, you need the following Python libraries:

- `opencv-python`
- `numpy`
- `mediapipe`
- `tensorflow`
- `pyttsx3`

You can install these dependencies using the following command:

```bash
pip install opencv-python numpy mediapipe tensorflow pyttsx3
```

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/sign-language-detection.git
   cd sign-language-detection
   ```

2. **Run the Script**:
   ```bash
   python sign_language_detection.py
   ```

3. **Interact with the System**:
   - The system will open a window showing the live video feed from your webcam.
   - Perform hand gestures corresponding to the letters A-Z.
   - The predicted letter will be displayed on the screen.
   - Press the `S` key to store the current letter and add it to the final word.
   - When the hand is no longer visible, the system will speak the stored word.
   - Press the `Q` key to quit the application.

## Code Overview

### Key Components

- **Hand Landmark Extraction**: The `extract_hand_landmarks` function processes the video frame to detect hand landmarks using MediaPipe.
- **Model Prediction**: The pre-trained TensorFlow model predicts the letter corresponding to the detected hand gesture.
- **Text-to-Speech**: The `pyttsx3` library is used to convert the stored word into speech.
- **User Interaction**: The system allows users to manually store letters and form words by pressing the `S` key.

## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

- **MediaPipe**: For providing the hand landmark detection model.
- **TensorFlow**: For the deep learning framework.
- **pyttsx3**: For the text-to-speech functionality.
