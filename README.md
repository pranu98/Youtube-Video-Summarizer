Speech-To-Text Transcription and Summarization Web Application
This project develops a web application that enables users to upload videos or provide video links to automatically transcribe audio into text. The application also offers translation options and generates a concise summary of the video’s content. Built using the Flask framework, it leverages OpenAI’s Whisper model for transcription, the BART-Large model for summarization, and the PyTube library for video downloading.

🚀 Key Components
🎥 Video Downloader: Downloads videos from YouTube or accepts video files uploaded by the user using the PyTube library.
💬 Subtitle Generator: Transcribes video audio using OpenAI's Whisper model with translation capabilities.
📝 Summarizer: Summarizes the transcribed text using the BART-Large model.
🌐 Deployment
Containerization: The application is packaged with Docker to ensure consistency across environments.
CI/CD: CircleCI automates building, testing, and deploying the application to AWS EC2, ensuring continuous integration and deployment.
🛠️ How to Run?
Clone the Repository:
bash
Copy code
git clone <repository-link>
Set Up Environment:
bash
Copy code
conda create -p env python=3.10 -y
conda activate env
Install Dependencies:
bash
Copy code
pip install -r requirements.txt
Run the Application:
bash
Copy code
python app.py
Access the Application:
Open http://localhost:5000 in your browser.
🐳 Run Locally with Docker
Build the Docker Image:
bash
Copy code
docker build -t vsum .
Run the Docker Container:
bash
Copy code
docker run -d -p 8080:8080 <IMAGEID>
👨‍💻 Tech Stack Used
Python
Flask
PyTorch
Docker
Transformers
🌐 Infrastructure Required
AWS EC2
AWS ECR
CircleCI
📂 Project Structure
The main package folder is videosum, containing all essential components.
🔍 Conclusion
This application streamlines the process of transcribing, translating, and summarizing video content, with potential improvements including advanced NLP techniques for enhanced accuracy and broader language support. It has wide-ranging applications in entertainment, education, business, and accessibility for individuals with hearing impairments.
