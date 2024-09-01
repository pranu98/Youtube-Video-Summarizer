# **Speech-To-Text Transcription and Summarization Web Application**

This project develops a web application that enables users to upload videos or provide video links to automatically transcribe audio into text. The application also offers translation options and generates a concise summary of the video’s content. Built using the Flask framework, it leverages OpenAI’s Whisper model for transcription, the BART-Large model for summarization, and the PyTube library for video downloading.

### 🚀 **Key Components**
- **🎥 Video Downloader**: Downloads videos from YouTube or accepts video files uploaded by the user using the `PyTube` library.
- **💬 Subtitle Generator**: Transcribes video audio using `OpenAI's Whisper model` with translation capabilities.
- **📝 Summarizer**: Summarizes the transcribed text using the `BART-Large model`.

### 🌐 **Deployment**
- **Containerization**: The application is packaged with `Docker` to ensure consistency across environments.
- **CI/CD**: `CircleCI` automates building, testing, and deploying the application to `AWS EC2`, ensuring continuous integration and deployment.

### 🛠️ **How to Run?**
1. **Clone the Repository**:
   ```bash
   git clone <repository-link>

