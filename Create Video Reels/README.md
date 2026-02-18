# Create Video Reels

An n8n workflow that automates the creation of video reels from product images using Generative AI.

## 🚀 Features

- **Form Trigger**: Starts with a user submission containing product details (Subject, Environment, Outfit, Lighting, etc.) and an image.
- **Image Analysis**: Uses Google Gemini to analyze the uploaded product image.
- **Prompt Engineering**:
   - Generates an optimized image generation prompt.
   - Creates a "flirty" or engaging text caption for the post.
   - Crafts a detailed video generation prompt.
- **Video Generation**: Uses Kling AI (via Fal.ai) to turn the image and prompt into a video.
- **Google Sheets**: Logs all data (photos, videos, descriptions) to Google Sheets.

## 🛠️ How It Works

1. **Input**: User fills a form with product details and uploads an image.
2. **Analyze**: Gemini Vision analyzes the image context.
3. **Generate Assets**:
   - **New Image Prompt**: Based on analysis and user edits.
   - **Video Prompt**: Optimized for cinematic motion.
   - **Caption**: Engaging text for social media.
4. **Create Video**: Calls the Fal.ai API to generate the video on Kling.
5. **Save**: Appends links and text to Google Sheets for review.

## ⚙️ Setup

1. **Import Workflow**: Load the `.json` file into n8n.
2. **Credentials Needed**:
   - **Google Gemini (PaLM) API**: For image analysis.
   - **OpenAI API**: For prompt generation.
   - **Fal.ai API (OpenRouter/Other)**: For video generation.
   - **Cloudinary**: For image hosting/uploading.
   - **Google Sheets**: For data logging.
