# 🎨 AdSnap Studio

AdSnap Studio is a Streamlit web app for creating professional product ads with AI. It connects to [Bria AI](https://bria.ai)'s image APIs, so you can go from a text prompt or a plain product photo to ad-ready visuals in a few clicks.


## 🌟 Features

- 🖼️ **Text-to-image:** generate HD product images with custom aspect ratio (1:1, 16:9, 9:16, 4:3, 3:4), style and 1–4 results
- ✨ **Prompt enhancement:** let AI improve your prompt before generating
- 🎯 **Packshots:** remove backgrounds and set a custom background color
- 🌅 **Shadows:** add realistic shadows with adjustable intensity, blur and offset
- 🏠 **Lifestyle shots:** place your product in a scene from a text description or a reference image
- 🎨 **Generative fill:** draw a mask on an image and fill it with AI-generated content
- 🧹 **Erase elements:** remove objects or the foreground
- 💾 **Download** any result

## 🛠️ Tech Stack

Python · Streamlit · Bria AI API · Pillow · Requests

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/Piyushkc241/adsnap-studio.git
cd adsnap-studio
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Get an API key from [Bria AI](https://bria.ai) and create a `.env` file in the root directory (see `.env.example`):
```
BRIA_API_KEY=your_api_key_here
```

4. Run the app:
```bash
python -m streamlit run app.py
```

## 💡 Usage

The app has four tabs:

| Tab | What it does |
|-----|--------------|
| **Generate Image** | Enter a prompt (optionally enhance it), choose aspect ratio and style, and generate images |
| **Product Photography** | Upload a product photo, then create a packshot, add a shadow, or generate a lifestyle shot |
| **Generative Fill** | Upload an image, draw a mask, and describe what should appear there |
| **Erase Elements** | Upload an image and remove unwanted elements |

## 📁 Project Structure

```
app.py          # Streamlit UI and tabs
services/       # One module per Bria API (generation, shadow, packshot, lifestyle, fill, erase)
workflows/      # Chained ad-generation pipeline
components/     # Reusable UI pieces (sidebar, uploader, preview)
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Bria AI](https://bria.ai) for the image generation APIs
- [Streamlit](https://streamlit.io) for the web framework
