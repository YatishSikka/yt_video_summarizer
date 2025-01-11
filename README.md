# YouTube Video Summarizer
YouTube Video Summarizer built using open source LLM and Framework like Llama 2, Haystack, Whisper, and Streamlit. This app smoothly runs on CPU as Llama 2 model is in GGUF format loaded through Llama.cpp.

## Description:
YouTube Video Summarizer, is a powerful and customizable tool at your disposal, capable of automatically summarizing YouTube videos. 

## **Features**
- **Transcription**: Uses OpenAI's `Whisper` model for accurate transcription of video content.
- **Summarization**: Utilizes LLaMA 2-7B-32K open-source model for high-quality summarization.
- **Interactive UI**: Built with `Streamlit` for a user-friendly experience.
- **Privacy**: Runs locally, ensuring no data is sent to external servers.

---

## **Technologies Used**
- **LLaMA 2-7B-32K (GGUF format)**: A local LLaMA model quantized for efficient inference using `llama-cpp`.
- **Whisper**: For transcribing audio to text.
- **Haystack**: For document processing and query-based summarization.
- **Streamlit**: For the interactive web application.

---

## **Prerequisites**
1. Python 3.8+ installed.
2. A CUDA-compatible GPU (optional but recommended for faster inference).
3. Required libraries installed.

---

## **Installation**
Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```

---

## Usage/Examples

1. Run the Streamlit app by executing:
```bash
streamlit run yt_summary.py

```

2.The web app will open in your browser.
- Copy and paste the YouTube video URL in the URL field and click on Submit.
- Since it is a local implementation of llama model, it will take a couple of minutes for processing.
- After processing, the summary will be displayed alongside the youtube video in the Streamlit interface.

---

## Project Structure

- yt_summary.py: The main Streamlit application script, containing all the functions for each step.
- model_add.py: It creates a custom Llama CPP InvocationLayer Instance with 32k max_length.
- requirements.txt: A list of required Python packages for the project.
