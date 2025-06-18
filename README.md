## Emotion-Detection-using-AWS-Rekognition

This web application uses **AWS Rekognition** to detect faces and emotions in images uploaded by the user or captured via their webcam. It leverages the power of **AWS Rekognition's facial analysis** and **emotion detection** features to analyze images and return information about emotions such as happiness, sadness, anger, etc.

### Features:
- **Capture from Camera**: Users can capture an image using their webcam, which will then be processed for face detection and emotion analysis.
- **Upload Image**: Users can upload an image from their device, which will be processed using AWS Rekognition for face and emotion detection.
- **Real-Time Results**: After processing, the application displays the image with bounding boxes around detected faces, along with the identified emotions.
- **AWS Rekognition Integration**: The application uses **AWS Rekognition API** for detecting faces and analyzing emotions from the images.

### Technologies Used:
- **Flask**: A lightweight Python web framework used to build the web application.
- **AWS Rekognition**: Cloud-based AI service for facial recognition and emotion detection.
- **HTML, CSS, and JavaScript**: For building the user interface and enabling real-time camera access.
- **Python Imaging Library (PIL)**: Used to draw bounding boxes around faces and display detected emotions on the images.

### Installation Instructions:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Jay-Ryali-11/Emotion-Detection-using-AWS-Rekognition.git
   ```

2. **Set Up Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure AWS Credentials**:
   - Set up your AWS credentials using the AWS CLI:
     ```bash
     aws configure
     ```
   - Alternatively, you can manually input your credentials in the Python script (not recommended for production).

5. **Run the Flask Application**:
   ```bash
   python app.py
   ```

6. **Access the Application**:
   Open your browser and go to `http://127.0.0.1:8080` to use the application.

### Notes:
- This project uses **AWS Rekognition**, which requires an AWS account. Make sure you have the correct **IAM permissions** to access the Rekognition API (e.g., `rekognition:DetectFaces`).
- The credentials (`aws_access_key_id`, `aws_secret_access_key`) need to be configured for the Rekognition API to function properly.
  
---
