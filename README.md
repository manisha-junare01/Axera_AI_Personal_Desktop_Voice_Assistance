# 🤖 Axera AI – Your Personal Voice Assistant

**Axera AI** is a smart personal desktop voice assistant built using Python and modern AI tools.
It helps users automate daily computer tasks, interact with apps via speech, and integrate with APIs like Google Calendar, ChatGPT, and more.

---

## 🌟 Key Features

✅ Wake word activation
✅ Voice authentication (male/female voice switch)
✅ System & media control (shutdown, volume, play/pause)
✅ App and web automation (Notepad, YouTube, Chrome)
✅ Email & WhatsApp messaging
✅ Wikipedia & Google Search
✅ Word-to-number calculator (BODMAS)
✅ PDF reader, notes, reminders, alarms
✅ Google Calendar integration
✅ Local and Spotify/YouTube music control
✅ ChatGPT-powered AI interaction
✅ Weather, news, battery & brightness updates
✅ Multi-language support (Marathi, Hinglish, English)
✅ Offline basic commands
✅ Logging, memory, and error handling

---

## 🧠 Tech Stack

**Language:** Python
**Libraries:** `speech_recognition`, `pyttsx3`, `pyaudio`, `pywhatkit`, `wikipedia`, `smtplib`, `requests`, `schedule`, `opencv`, `Pillow`, `psutil`, `googletrans`, `openai`, `tkinter`
**Build Tools:** `PyInstaller`, `Inno Setup`
**Frontend (Website):** HTML, CSS, JS (or React + Tailwind)

---

## 🛠️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/Axera-AI.git
cd Axera-AI
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Assistant

```bash
python src/main.py
```

### 4️⃣ Build Executable

```bash
pyinstaller --onefile --windowed --icon=setup/icon.ico src/main.py
```

Use **Inno Setup** to create installer and shortcut for desktop use.

---

## 🔐 Login + Voice Authentication Flow

* User registers → enters name, sets voice password
* System trains voiceprint (using `speech_recognition` + `pyaudio`)
* On startup → waits for **wake word ("Axera")**
* Authenticates user → activates assistant

---

## 📁 Website Pages

* **Home** – Overview & download button
* **Download** – Installer + setup guide
* **How to Use** – Step-by-step with screenshots
* **About/Team** – Developers & project vision
* **Contact** – Email, GitHub, Support form

---

## 🧩 Project Modules

| Module              | Description                     |
| ------------------- | ------------------------------- |
| `voice_engine.py`   | Speech recognition + synthesis  |
| `auth.py`           | User login + voice verification |
| `ai_chat.py`        | ChatGPT integration             |
| `scheduler.py`      | Alarms + reminders              |
| `system_control.py` | System, media & app controls    |
| `pdf_reader.py`     | PDF to speech                   |
| `music_player.py`   | Local & online music control    |
| `camera_control.py` | Camera open/capture             |
| `calculator.py`     | BODMAS calculator               |
| `gui.py`            | Tkinter-based dashboard         |

---

## ⚙️ Troubleshooting

| Issue                  | Solution                                     |
| ---------------------- | -------------------------------------------- |
| Mic not detected       | Check `pyaudio` installation                 |
| Wake word not working  | Retrain voice or check noise levels          |
| No sound output        | Change default output device                 |
| ChatGPT not responding | Check API key in `.env`                      |
| Installer failed       | Run as admin / disable antivirus temporarily |

---

## 📜 License

This project is licensed under the MIT License.

---

## 👩‍💻 Team

**Axera AI** by

* Manisha Junare (Lead Developer)
* Shraddha Salve
* Yutee Kharat-Patil
* Abhishek Bankar

---

## 💌 Contact

📧 [manishajunare@gmail.com](mailto:manishajunare@gmail.com)
🌐 [GitHub Repository](https://github.com/yourusername/Axera-AI)
