# AI_Nutritionist_using_YOLO_GEMINI

# Diet Analysis with Image Recognition

This project uses computer vision and generative AI to analyze meal images and provide personalized nutrition information.

## Features

- Object detection using YOLOv8 to identify food items in uploaded images
- Nutrition estimation using Google's Gemini AI model
- Personalized macronutrient breakdown based on user details
- RDA (Recommended Dietary Allowance) analysis and dietary suggestions
- User-friendly interface built with Gradio

## Requirements

- Python 3.7+
- Ultralytics YOLOv8
- Google Generative AI
- Gradio
- Pillow
- OpenCV
- Matplotlib

## Setup

1. Install required packages:
   ```
   pip install gradio ultralytics google-generativeai pillow opencv-python matplotlib
   ```

2. Set up environment variables:
   - `GEMINI_API_KEY`: Your Google Gemini API key
   - `YOLO_MODEL_PATH`: Path to your custom YOLOv8 model file

3. Ensure you have a trained YOLOv8 model for food detection

## Usage

1. Run the script:
   ```
   python diet_analysis.py
   ```

2. Open the Gradio interface in your web browser

3. Upload an image of a meal

4. Enter your personal details (height, weight, age, sex, diet type)

5. Submit and view the analysis results

## How It Works

1. The uploaded image is processed using a YOLOv8 model to detect food items
2. The detected food item is cropped from the original image
3. Google's Gemini AI analyzes the cropped image to estimate nutrition information
4. Based on user details, a personalized macronutrient breakdown is generated
5. An RDA analysis is performed, providing dietary suggestions

## Customization

- Modify the prompts in the `process_image` function to adjust the AI's output
- Update the Gradio interface in the `gradio_interface` function to change the UI



## Acknowledgements

- Ultralytics for YOLOv8
- Google for the Gemini AI model
- Gradio for the web interface

This README provides an overview of the project, its features, setup instructions, and how it works. You may want to add more details about the specific YOLOv8 model used, any data preprocessing steps, or additional configuration options.

