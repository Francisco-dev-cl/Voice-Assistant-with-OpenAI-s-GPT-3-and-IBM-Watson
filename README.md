# Voice Assistant with OpenAI's GPT-3 and IBM Watson

This repository contains a full-stack project implementing an intelligent conversational voice assistant that integrates advanced speech processing services with OpenAI's generative language model.

## 🎯 Project Objective

The goal of this application is to orchestrate a complete voice-to-voice pipeline. It processes incoming audio recordings, converts spoken words to text, sends the text payload to an LLM to generate a contextual answer, and synthesizes the final output text back into natural-sounding speech.

## 📁 Repository Structure

* **`server.py`**: The application's main backend web server, establishing endpoints for interface navigation and processing raw multimedia network requests.
* **`worker.py`**: The background processing module responsible for coordinating core pipeline tasks like service authentications and external API streaming requests.
* **`templates/`**: Presentation files organizing the visual application interface layout within the user's web browser.
* **`static/`**: Hosts assets that control client-side operations, style layouts, and audio-capture recording interfaces.
* **`models/`**: Dedicated repository folder for housing configuration parameters, prompt structures, or auxiliary machine learning artifacts.
* **`Dockerfile`**: A unified containerization template mapping out the environment dependencies for standardized cloud distribution.
* **`requirements.txt`**: Complete Python package manifest locking down the libraries needed to run the ecosystem safely.

## 🛠 Technologies Used

* **Orchestration & Backend:** Python 3.x, Flask
* **Cognitive Services:** IBM Watson (Speech to Text / Text to Speech)
* **Generative Intelligence:** OpenAI API (GPT-3/Text-Generation architectures)
* **Environment & Containerization:** Docker
* **Frontend Components:** HTML5, CSS3, JavaScript (Media Stream Recording API)

## 🚀 Installation and Execution

### Local Environment Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd Voice-Assistant-with-OpenAI-s-GPT-3-and-IBM-Watson
   ```

2. **Install project dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Start the backend server:**
   ```bash
   python server.py
   ```

### Running with Docker Containers

To stand up the application without manual package matching:

1. **Assemble the Docker image:**
   ```bash
   docker build -t voice-assistant-app .
   ```

2. **Spin up the isolated container:**
   ```bash
   docker run -p 5000:5000 voice-assistant-app
   ```

## 📈 Demonstrated Skills

* **Multimodal API Integration:** Connecting independent third-party ecosystems (OpenAI + IBM Watson) into a unified, low-latency audio transaction loop.
* **Asynchronous Task Architecture:** Offloading heavy cognitive processing or remote network requests via dedicated execution patterns (`worker.py`) to keep the primary UI responsive.
* **Cloud Infrastructure Prep:** Architecting immutable multi-stage `Dockerfiles` capable of securely wrapping sensitive API integrations for immediate web deployment.
