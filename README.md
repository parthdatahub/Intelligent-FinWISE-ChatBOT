# Intelligent FinWISE AI ChatBOT Application

This repository contains the source code for the **Intelligent FinWISE AI ChatBOT**, an application designed to handle financial data queries and user interactions using AI and Google Cloud Platform (GCP) services.

## Features
- Dialogflow CX for chatbot conversation flow.
- Integration with Gemini AI for advanced query resolution.
- Financial data handling and dynamic response generation.
- Scalable deployment using Docker and Cloud Run.
- Document parsing and semantic search using embeddings.

## Tech Stack
- **Programming**: Python, Flask
- **Cloud Platform**: Google Cloud Platform (GCP)
- **APIs/Services**: Dialogflow CX, Cloud Run, Cloud Storage, Firestore, Cloud Functions
- **Databases**: Firestore, BigQuery
- **AI/ML Models**: Gemini AI, Word Embedding Models

## Installation and Setup
Follow these steps to set up the project locally or deploy on GCP:

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Intelligent-FinWISE-ChatBOT.git
   cd Intelligent-FinWISE-ChatBOT

2. Install required dependencies:
pip install -r requirements.txt

3. Run the Flask app:
python main.py


4. Deployment
Build the Docker image:
docker build -t flask-app .

5. Run the container locally:
docker run -p 8080:8080 flask-app

6. Deploy to Cloud Run:
gcloud run deploy flask-app \
  --image gcr.io/<PROJECT_ID>/flask-app \
  --platform managed \
  --region us-central1 \
  --allow-unauthenticated

7. Directory Structure

Intelligent-FinWISE-ChatBOT/

|-- main.py             # Flask application entry point
|-- requirements.txt    # Python dependencies
|-- Dockerfile          # Docker image configuration
|-- README.md           # Project documentation
|-- templates/          # HTML templates for the Flask app
|-- static/             # Static files (CSS, JS, images)


