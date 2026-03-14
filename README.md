# Podcast Generator
An AI-powered tool that automates the creation of high-quality podcasts. This project leverages Large Language Models (LLMs) to generate engaging conversational scripts and advanced Text-to-Speech (TTS) engines to produce lifelike audio content.

# Features
Automated Scriptwriting: Generates natural-sounding dialogue between multiple speakers based on a provided topic or source material.

Realistic Voice Synthesis: Uses state-of-the-art TTS (e.g., ElevenLabs or OpenAI) to create human-like voices with emotion and pacing.

RAG Integration: (Optional) Ability to upload PDFs or documents to ground the podcast in specific facts.

Audio Stitching: Automatically merges individual dialogue clips into a single, seamless MP3 file with realistic pauses.

Customizable Personalities: Configure different speaker roles (Host, Expert, Skeptic) to vary the tone of the conversation.

# Tech Stack
Language: Python 3.10+

AI Models: OpenAI (GPT-4o), ElevenLabs API

Processing: LlamaIndex (for data retrieval), PyDub (for audio manipulation)

Interface: Gradio / Streamlit (if applicable)

# Prerequisites
Before you begin, ensure you have the following:

Python installed.

An OpenAI API Key and/or ElevenLabs API Key.

FFmpeg installed on your system (required for audio processing).

# Installation
Clone the repository:

Bash
git clone https://github.com/EthanJackson1/podcast-generator.git
cd podcast-generator
Create a virtual environment:

Bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
Install dependencies:

Bash
pip install -r requirements.txt
Environment Variables:
Create a .env file in the root directory and add your API keys:

Code snippet
OPENAI_API_KEY=your_key_here
ELEVENLABS_API_KEY=your_key_here

# Usage
Run the main script to start generating your podcast:

Bash
python main.py
Follow the on-screen prompts to enter your topic or upload the documents you want the podcast to discuss.

# Project Structure
Plaintext
.
├── src/                # Source code
├── data/               # Input documents (PDFs/Text)
├── output/             # Generated MP3 files and scripts
├── requirements.txt    # Python dependencies
├── .env                # API keys (hidden)
└── main.py             # Entry point

# Contributing
Contributions are welcome! If you have ideas for new features or improvements, please:

Fork the Project.

Create your Feature Branch (git checkout -b feature/AmazingFeature).

Commit your Changes (git commit -m 'Add some AmazingFeature').

Push to the Branch (git push origin feature/AmazingFeature).

Open a Pull Request.

# License
Distributed under the MIT License. See LICENSE for more information.
