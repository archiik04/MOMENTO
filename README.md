# AI Video Generator

An affordable AI-powered video generation platform that's **85-95% cheaper than expected SORA pricing**. Automatically create professional videos with AI-generated scripts, narration, visuals, and subtitles.

## 🎯 Features

### Core Capabilities
- **AI Script Generation**: Generate video scripts with narration and visual descriptions using GPT-4
- **Automated Video Creation**: Create synchronized videos from folders of images and audio clips
- **Subtitle Integration**: Embed subtitles directly in videos with SRT file support
- **Intro/Outro Customization**: Add branded intro and outro clips with customizable topics and backgrounds
- **Visual Effects**: Apply professional transitions including fade-in and fade-out effects
- **Multi-Format Support**: Work with various media formats (images, audio, video)

### Advanced Features
- **Content Extraction**: Extract and process content from JSON, PDF, and PPTX files
- **AI Image Generation**: Generate custom visuals using OpenAI DALL-E
- **Neural Text-to-Speech**: High-quality voice synthesis with Kokoro TTS
- **Activity Recognition**: Intelligent scene analysis using Hugging Face transformers

## 🛠️ Tech Stack

### Backend
- **Flask** - Web framework
- **Flask-CORS** - Cross-origin resource sharing
- **Flask-SQLAlchemy** - Database ORM

### Video & Audio Processing
- **MoviePy** - Video editing and composition
- **PySRT** - Subtitle file handling
- **Pillow (PIL)** - Image processing
- **SoundFile** - Audio file handling

### AI & Machine Learning
- **OpenAI GPT-4** - Script generation
- **Google Gemini** - Roadmap generation
- **Hugging Face Transformers** - Pre-trained models
- **PyTorch** - Deep learning framework
- **Kokoro TTS** - Text-to-speech synthesis
- **DALL-E** - AI image generation

### File Processing
- **PyMuPDF (fitz)** - PDF text extraction
- **python-pptx** - PowerPoint processing
- **BeautifulSoup4** - Web scraping
- **Requests** - HTTP requests

## 📋 Prerequisites

- Python 3.8+
- OpenAI API key
- Google Generative AI API key
- FFmpeg (for video processing)


### Basic Video Generation

```python
# Generate a script and create a video
from video_generator import generate_video

video_path = generate_video(
    topic="Introduction to AI",
    duration=60,
    include_subtitles=True
)
```

### Custom Video with Assets

```python
# Create video from existing images and audio
from video_generator import create_from_assets

video_path = create_from_assets(
    images_folder="./assets/images",
    audio_folder="./assets/audio",
    output_path="./output/custom_video.mp4"
)
```

## 🎬 Workflow

1. **Script Generation**: AI generates narration and visual descriptions
2. **Asset Creation**: Generate or use existing images and audio
3. **Video Assembly**: Synchronize visuals with audio using MoviePy
4. **Subtitle Generation**: Create and embed SRT subtitles
5. **Post-Processing**: Apply effects and add intro/outro



## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenAI for GPT-4 and DALL-E APIs
- Google for Generative AI (Gemini)
- Kokoro TTS for text-to-speech synthesis
- MoviePy for video processing capabilities

## 📧 Contact

For questions or support, please open an issue on GitHub.

---

**Note**: API costs apply when using OpenAI and Google AI services. Monitor your usage to stay within budget.
