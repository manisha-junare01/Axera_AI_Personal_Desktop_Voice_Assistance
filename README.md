# 🎙️ Axera AI - Personal Voice Assistant

<div align="center">

![Axera AI Logo](assets/images/logo.png)

**Your Intelligent Desktop Companion**

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-blue.svg)](https://www.microsoft.com/windows)
[![Stars](https://img.shields.io/github/stars/yourusername/axera-ai?style=social)](https://github.com/yourusername/axera-ai)

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Documentation](#-documentation) • [Contributing](#-contributing)

</div>

---

## 📖 Overview

**Axera AI** is an advanced, open-source personal voice assistant for desktop computers. Built with Python, it provides comprehensive hands-free control over your system, integrates with popular applications, and leverages AI for intelligent conversations.

Unlike cloud-based assistants, Axera AI prioritizes **privacy**, **customization**, and **local control** while offering powerful features through seamless API integrations.

### 🎯 Key Highlights

- 🎤 **Wake Word Activation** - Just say "Hey Assistant"
- 🔐 **Voice Authentication** - Secure access with your voice
- 🖥️ **Complete System Control** - Manage your computer hands-free
- 🤖 **AI-Powered** - Natural conversations with ChatGPT integration
- 🌐 **Offline Capable** - Basic commands work without internet
- 🎨 **Modern GUI** - Beautiful, intuitive interface
- 🔧 **Highly Customizable** - Extensible architecture
- 🔒 **Privacy-Focused** - Your data stays on your device

---

## ✨ Features

### 🎯 Core Capabilities

<table>
<tr>
<td width="50%">

#### 🖥️ System Control
- Shutdown, restart, lock, sleep
- Volume control (up, down, mute)
- Screen brightness adjustment
- Window management
- Battery status monitoring

#### 🎵 Media Management
- Local music playback
- Spotify integration
- YouTube Music control
- Play, pause, next, previous
- Volume control

</td>
<td width="50%">

#### 🌐 Web & Apps
- Open/close applications
- Web searches (Google, YouTube)
- Wikipedia queries
- Website launching
- Browser control

#### 💬 Communication
- WhatsApp messaging
- Email sending
- Voice-based composition
- Quick messaging

</td>
</tr>
<tr>
<td width="50%">

#### 📝 Productivity
- Note taking
- Reminders & alarms
- Google Calendar integration
- PDF reading
- Screenshot capture
- Camera control

#### 🤖 AI Features
- Natural conversations (ChatGPT)
- Question answering
- Code assistance
- Jokes & compliments
- Learning user preferences

</td>
<td width="50%">

#### 🌍 Information
- Real-time weather updates
- Latest news headlines
- Wikipedia summaries
- Calculator (voice-based)
- Translation support

#### 🔐 Security
- Voice authentication
- Secure API key storage
- Privacy-focused design
- Local data processing

</td>
</tr>
</table>

---

## 🚀 Quick Start

### Prerequisites

- **OS:** Windows 10/11 (64-bit)
- **Python:** 3.8 or higher
- **Microphone:** Any USB or built-in mic
- **Internet:** For AI and web features

### Installation

#### Option 1: Download Installer (Recommended)

1. Download the latest `AxeraAI-Setup.exe` from [Releases](https://github.com/yourusername/axera-ai/releases)
2. Run the installer as Administrator
3. Follow the setup wizard
4. Launch Axera AI from desktop shortcut

#### Option 2: Build from Source

```bash
# Clone the repository
git clone https://github.com/yourusername/axera-ai.git
cd axera-ai

# Create virtual environment
python -m venv venv
venv\Scripts\activate  # On Windows

# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py
```

---

## 🎮 Usage

### First Time Setup

1. **Launch Axera AI**
2. **Complete Voice Registration**
   - Speak your name when prompted
   - Record voice samples for authentication
3. **Configure API Keys** (Optional but recommended)
   - OpenAI API for ChatGPT features
   - Picovoice key for wake word detection
   - Weather and News API keys

### Basic Commands

```
🎤 Wake Word: "Hey Assistant"

💻 System Control:
  "Shutdown computer"
  "Restart system"
  "Lock screen"
  "Increase volume"
  "Decrease brightness"

🌐 Applications & Web:
  "Open Chrome"
  "Close Notepad"
  "Search YouTube for music"
  "Search Google for Python tutorials"

🎵 Media:
  "Play music"
  "Pause"
  "Next song"
  "Play [song name] on Spotify"

📝 Productivity:
  "Take a note saying [your note]"
  "Set reminder for 5 minutes"
  "Set alarm for 7 AM"
  "What's on my calendar?"

ℹ️ Information:
  "What's the weather?"
  "Latest news"
  "Wikipedia search for artificial intelligence"
  "Calculate 25 times 4"

🤖 AI Chat:
  "Tell me a joke"
  "What is quantum computing?"
  "Help me write a function"
  "Explain machine learning"

🛑 Exit:
  "Exit"
  "Goodbye"
  "Stop"
```

---

## ⚙️ Configuration

### API Keys Setup

Edit `config.json` or use the Settings panel:

```json
{
  "openai_api_key": "sk-your-openai-key",
  "picovoice_access_key": "your-picovoice-key",
  "weather_api_key": "your-weather-key",
  "news_api_key": "your-news-key",
  "spotify_client_id": "your-spotify-id",
  "spotify_client_secret": "your-spotify-secret"
}
```

### Getting API Keys

| Service | Link | Free Tier |
|---------|------|-----------|
| OpenAI | [platform.openai.com](https://platform.openai.com/) | $5 credit |
| Picovoice | [console.picovoice.ai](https://console.picovoice.ai/) | Free |
| OpenWeather | [openweathermap.org/api](https://openweathermap.org/api) | Free |
| News API | [newsapi.org](https://newsapi.org/) | Free |
| Spotify | [developer.spotify.com](https://developer.spotify.com/dashboard) | Free |

### Customization

**Change Voice:**
```json
{
  "voice_type": "male" or "female",
  "voice_rate": 175,
  "voice_volume": 0.9
}
```

**Change Wake Word:**
```json
{
  "wake_word": "Hey Assistant"  // or custom phrase
}
```

**Language Support:**
```json
{
  "language": "en-IN"  // en-US, hi-IN, mr-IN
}
```

---

## 📁 Project Structure

```
AxeraAI/
├── main.py                      # Main application entry
├── requirements.txt             # Python dependencies
├── config.json                  # Configuration file
├── README.md                    # This file
│
├── modules/                     # Core modules
│   ├── __init__.py
│   ├── voice_engine.py          # Speech recognition & TTS
│   ├── wake_word.py             # Wake word detection
│   ├── authenticator.py         # Voice authentication
│   ├── system_controller.py     # System operations
│   ├── media_controller.py      # Media control
│   ├── web_controller.py        # Web & app control
│   ├── communication.py         # Messaging
│   ├── productivity.py          # Productivity tools
│   ├── ai_brain.py              # AI integration
│   ├── gui.py                   # GUI interface
│   └── config_manager.py        # Configuration management
│
├── assets/                      # Resources
│   ├── icons/                   # Application icons
│   ├── sounds/                  # Audio files
│   └── images/                  # Images
│
├── data/                        # User data
│   ├── users/                   # User profiles
│   ├── notes/                   # Notes
│   └── reminders/               # Reminders
│
├── logs/                        # Application logs
│
├── tests/                       # Unit tests
│   └── test_modules.py
│
└── build/                       # Build files
    ├── axera.spec               # PyInstaller spec
    └── installer.iss            # Inno Setup script
```

---

## 🛠️ Development

### Building from Source

```bash
# Install development dependencies
pip install -r requirements-dev.txt

# Run tests
python -m pytest tests/

# Build executable
pyinstaller axera.spec

# Create installer (requires Inno Setup)
iscc build/installer.iss
```

### Adding New Features

1. Create new module in `modules/`
2. Implement required methods
3. Register command patterns in `main.py`
4. Add tests in `tests/`
5. Update documentation

**Example: Adding a New Command**

```python
# In main.py
def _execute_command(self, command):
    command_lower = command.lower()
    
    # Add your new command
    if 'your new command' in command_lower:
        return self.your_controller.your_method(command)
```

---

## 🧪 Testing

### Running Tests

```bash
# Run all tests
python -m pytest tests/ -v

# Run specific test
python -m pytest tests/test_voice_engine.py

# Run with coverage
python -m pytest tests/ --cov=modules
```

### Manual Testing

Use the provided test checklist:
- [ ] Wake word detection
- [ ] Voice authentication
- [ ] System commands
- [ ] Media control
- [ ] Web searches
- [ ] AI responses
- [ ] GUI functionality

---

## 📚 Documentation

- **[User Manual](docs/USER_MANUAL.md)** - Complete usage guide
- **[API Reference](docs/API_REFERENCE.md)** - Module documentation
- **[Developer Guide](docs/DEVELOPER_GUIDE.md)** - Contributing guide
- **[Troubleshooting](docs/TROUBLESHOOTING.md)** - Common issues
- **[FAQ](docs/FAQ.md)** - Frequently asked questions

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Ways to Contribute

- 🐛 **Report Bugs** - Create detailed issue reports
- 💡 **Suggest Features** - Share your ideas
- 📝 **Improve Documentation** - Help others understand
- 🔧 **Submit Pull Requests** - Add new features or fix bugs
- ⭐ **Star the Project** - Show your support

### Contribution Guidelines

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

---

## 🐛 Troubleshooting

### Common Issues

<details>
<summary><b>Microphone not detected</b></summary>

**Solutions:**
1. Check Windows Privacy Settings
2. Grant microphone permissions to Axera AI
3. Select correct input device in Sound Settings
4. Test microphone in other applications
</details>

<details>
<summary><b>Wake word not working</b></summary>

**Solutions:**
1. Verify Picovoice API key is configured
2. Reduce background noise
3. Speak clearly and directly at microphone
4. Check microphone sensitivity settings
5. Re-train wake word if necessary
</details>

<details>
<summary><b>Commands not executing</b></summary>

**Solutions:**
1. Check if required application is installed
2. Verify internet connection (for web commands)
3. Check logs: `%USERPROFILE%\AxeraAI\logs\`
4. Ensure proper permissions for system operations
</details>

<details>
<summary><b>API rate limits</b></summary>

**Solutions:**
1. Check your API usage on respective platforms
2. Upgrade to paid tier if needed
3. Reduce frequency of API calls
4. Use caching for repeated queries
</details>

For more issues, see [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md)

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| **Startup Time** | ~3.2 seconds |
| **Wake Word Latency** | <500ms |
| **Command Response** | 1.8s average |
| **Memory Usage** | ~180 MB |
| **CPU Usage** | 8-15% |
| **Recognition Accuracy** | ~88% |

*Tested on Intel Core i5, 8GB RAM, Windows 11*

---

## 🗺️ Roadmap

### Version 1.0 ✅ (Current)
- [x] Core voice assistant features
- [x] System control
- [x] AI integration
- [x] GUI interface
- [x] Windows support

### Version 1.5 (Q2 2025)
- [ ] macOS support
- [ ] Enhanced offline mode
- [ ] Plugin system
- [ ] Voice customization
- [ ] Emotion detection

### Version 2.0 (Q4 2025)
- [ ] Linux support
- [ ] Mobile companion app
- [ ] Smart home integration
- [ ] Cloud synchronization
- [ ] Multi-user support

### Version 3.0 (2026)
- [ ] AR/VR integration
- [ ] Predictive assistance
- [ ] Advanced AI models
- [ ] Enterprise features

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 🙏 Acknowledgments

- **OpenAI** - GPT-3.5 API for AI capabilities
- **Picovoice** - Porcupine wake word detection
- **Python Community** - Amazing libraries and tools
- **Contributors** - Everyone who helped improve this project

### Built With

- [Python](https://www.python.org/) - Programming language
- [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) - GUI framework
- [SpeechRecognition](https://github.com/Uberi/speech_recognition) - Speech recognition
- [pyttsx3](https://github.com/nateshmbhat/pyttsx3) - Text-to-speech
- [OpenAI API](https://openai.com/) - AI integration
- [Porcupine](https://picovoice.ai/) - Wake word detection

---

## 📞 Contact & Support

- **Developer:** [Manisha Junare]
- **Email:** manishajunare@gmail.com
- **Project Link:** [github.com/yourusername/axera-ai](https://github.com/yourusername/axera-ai)
- **Website:** [axeraai.com](https://axeraai.com)

### Community

- **Discord:** [Join our server](https://discord.gg/axeraai)
- **Twitter:** [@AxeraAI](https://twitter.com/axeraai)
- **Reddit:** [r/AxeraAI](https://reddit.com/r/axeraai)

---

## ⭐ Show Your Support

If you find Axera AI helpful, please consider:

- ⭐ **Star this repository**
- 🍴 **Fork and contribute**
- 📢 **Share with others**
- 💖 **Sponsor the project**

---

<div align="center">

**Made with ❤️ by Manisha**

[⬆ Back to Top](#-axera-ai---personal-voice-assistant)

</div>
