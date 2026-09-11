# YOLO Object Detection

A complete Python project that combines three AI capabilities in a single interactive chatbot:

- AI chat using the Groq API
- Object detection using Ultralytics YOLOv8
- OCR text extraction using EasyOCR

## Features

- Interactive menu-driven chatbot
- Multi-turn AI conversation with Groq
- Image-based object detection with YOLOv8
- Text extraction from images with EasyOCR
- Annotated output image saved in the output folder
- Extracted text saved to output/extracted_text.txt

## Project Structure

YOLO OBJECT DETECTION/
├── .venv
├── .env
├── chatbot.py
├── ocr.py
├── yolov8.py
├── yolov8n.pt
├── images.jpg
├── requirements.txt
├── README.md
└── output/

## Installation

### 1. Create a virtual environment

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

Linux/macOS:

```bash
python -m venv .venv
source .venv/bin/activate
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add your Groq API key

Open the .env file and replace the placeholder value:

```env
GROQ_API_KEY=your_api_key
```

## Run the Application

```bash
python main.py
```

## Example Output

```text
AI MULTI TOOL CHATBOT
1. Chat with AI
2. Detect Objects in Image
3. Read Text from Image (OCR)
4. About Project
5. Exit
```

## Troubleshooting

- If the YOLO model is missing, the script will try to download it automatically when possible.
- If EasyOCR fails on first run, it may download language models and take a few minutes.
- Ensure your Groq API key is valid and stored in the .env file.
- If you encounter dependency issues, recreate the virtual environment and reinstall requirements.
