# 🤖 Axera AI – Smart Desktop Voice Assistant

> Your personal AI-powered assistant built with Python 🧠✨

Axera is a **desktop voice assistant** that helps you perform everyday tasks — from playing music 🎵 and managing files 📂 to scheduling reminders 🕒, authenticating via voice 🔐, and chatting with AI 💬 — all through simple voice commands.

---

## 🚀 Features

### 🗣️ Voice Interaction

* Real-time **speech recognition & text-to-speech**
* **Wake word activation** (“Axera”)
* Switch between **male/female** voice

### 🪟 Modern GUI

* Built using **Tkinter** / **CustomTkinter**
* Status indicators (“Listening…”, “Processing…”)
* Start / Stop / Settings buttons
* Live mic animation + output command log

### 🔐 Authentication

* Register & login with **voice samples**
* Wake word detection for secure activation

### 🕒 Smart Scheduler

* **Reminders & alarms** with `schedule` + `datetime`
* Optional Google Calendar integration

### 📄 PDF Reader

* Reads PDF aloud using `PyPDF2` + `pyttsx3`

### 📸 Camera Control

* Open/close webcam
* Capture & save photos via `cv2`

### 🧮 Smart Calculator

* Understands natural language math (e.g. “five plus three”)
* Uses safe evaluation (BODMAS logic)

### 🎵 Music Player

* Play / Pause / Stop local files
* Play songs on **Spotify** or **YouTube** via `pywhatkit`

### ⚙️ System Control

* Adjust volume
* Shutdown / Restart / Lock system
* Window management using `pyautogui`

---

## 🧩 Folder Structure

```
AxeraAI/
│
├── main.py               # Entry point (controller)
├── voice_engine.py       # Voice input/output logic
├── gui.py                # GUI interface
├── auth.py               # Login & voice authentication
├── scheduler.py          # Reminders & Google Calendar
├── pdf_reader.py         # PDF reading aloud
├── camera_control.py     # Camera open/capture
├── calculator.py         # Word-based calculator
├── music_player.py       # Local & online music
├── system_control.py     # Volume & system commands
└── utils/                # Helper modules (if any)
```

---

## 🛠️ Tech Stack

| Area         | Tools / Libraries                          |
| ------------ | ------------------------------------------ |
| Language     | Python 3.x                                 |
| Voice Engine | `speech_recognition`, `pyttsx3`, `pyaudio` |
| GUI          | `tkinter`, `customtkinter`                 |
| AI Chat      | OpenAI API / ChatGPT                       |
| Camera       | `opencv-python`                            |
| PDF          | `PyPDF2`                                   |
| Scheduler    | `schedule`, `datetime`                     |
| System       | `os`, `pyautogui`, `pycaw`                 |

---

## ⚙️ Installation

1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/AxeraAI.git
cd AxeraAI
```

2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

3️⃣ Run the assistant

```bash
python main.py
```

---

## 🔊 Wake Word

Say **“Axera”** to activate your assistant.

Example commands:

* “Axera, open camera”
* “Axera, read my PDF”
* “Axera, play music”
* “Axera, remind me at 7 PM”

---

## 📸 Screenshots (Optional)

*(Add your GUI and demo images here)*

```
/assets/
├── gui_preview.png
├── voice_auth_demo.png
└── reminder_screenshot.png
```

---

## 👩‍💻 Author

**Manisha Junare**
📍 Pune, India
🌐 [LinkedIn](#) | [GitHub](#)

---

## 💡 Future Enhancements

* Add NLP-based smart conversation
* Integrate weather & news APIs
* Build cross-platform desktop app

---

## 🏁 License

This project is licensed under the **MIT License**.

---

✨ *Axera – “Think. Speak. Assist.”* ✨
