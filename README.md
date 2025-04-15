# YouTube Transcript to Detailed Notes Converter

This project is a web application that helps users convert YouTube video transcripts into easy-to-read, bullet-point summaries using Google Gemini AI. It's especially useful for students, professionals, or anyone who wants to quickly understand a video without watching the entire content.

---

## Features

- Accepts any valid YouTube video link.
- Automatically fetches the video transcript using YouTube Transcript API.
- Summarizes the transcript into key points using Google Gemini AI.
- Presents results in simple, clear bullet points.
- Built with Streamlit for an interactive and fast web interface.

---

## Technologies Used

- **Python** – Core programming language.
- **Streamlit** – For building the web interface.
- **YouTube Transcript API** – To extract transcript from YouTube videos.
- **Google Generative AI (Gemini)** – For generating summaries.
- **dotenv** – To manage API keys securely.

---

## How It Works

1. User enters a YouTube video link into the app.
2. The application extracts the video ID from the URL.
3. The transcript is fetched using the YouTube Transcript API.
4. A prompt is sent along with the transcript to the Gemini AI model.
5. The summary is generated and displayed as bullet points.

---

## Installation

### Step 1: Clone the repository

### Step 2: Install dependencies
```bash
pip install -r requirements.txt
```

Or manually:
```bash
pip install streamlit google-generativeai youtube-transcript-api python-dotenv
```

### Step 3: Add your API key
Create a `.env` file in the root directory and add your Google API key:
```
GOOGLE_API_KEY=your_google_gemini_api_key
```

---

## Running the App

```bash
streamlit run app.py
```

Then open the local link provided in your terminal to use the app in your browser.

---

## Folder Structure

```
YTTranscribe/
├── app.py                # Main Streamlit application
├── .env                  # Environment variables (not to be shared)
├── requirements.txt      # Required Python packages
```

---

## Future Improvements

- Download summary as PDF or text file
- Multi-language support
- Add timestamped highlights or topic segments
- Mobile-friendly UI
