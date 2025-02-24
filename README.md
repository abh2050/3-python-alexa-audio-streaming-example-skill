# Kantipur Radio Alexa Skill
![](https://is1-ssl.mzstatic.com/image/thumb/Purple116/v4/38/e9/9a/38e99aa6-3948-8d6c-c1a9-46e0fada4716/AppIcon-0-0-1x_U007emarketing-0-0-0-5-0-0-sRGB-0-0-0-GLES2_U002c0-512MB-85-220-0-0.jpeg/1200x630wa.png)

An Alexa skill that streams **Kantipur Radio**, Nepal's leading radio station, to Alexa-enabled devices.

## 📌 Description

This Alexa skill allows users to stream Kantipur Radio directly through their Alexa-enabled devices. The skill provides a simple interface to **play, pause, stop, and resume** the live radio stream with voice commands.

## 🎙️ Usage

To start listening to Kantipur Radio, simply say:

> **"Alexa, open Kantipur Radio"**

### 🔹 Voice Commands

| Command | Action |
|---------|--------|
| **"Alexa, open Kantipur Radio"** | Starts playing the live radio stream |
| **"Alexa, stop"** | Stops playback |
| **"Alexa, pause"** | Pauses the stream (if supported) |
| **"Alexa, resume"** | Resumes playback |
| **"Alexa, help"** | Provides skill-related assistance |
| **"Alexa, what is this?"** | Gives more information about the skill |

---

## 🌟 Features

- **Live Streaming:** Plays Kantipur Radio’s live stream 24/7.
- **Multi-Language Support:** Supports **en-US, en-GB, en-IN, en-AU, en-CA** locales.
- **Basic Playback Controls:** Includes play, pause, stop, and resume functionality.
- **Error Handling:** Graceful handling of connectivity and streaming issues.
- **Device Compatibility:** Works on Echo devices, Fire TV, and Alexa-enabled smart speakers.

---

## 🛠️ Tech Stack

| Component | Technology Used |
|-----------|----------------|
| **Programming Language** | Python |
| **Backend** | AWS Lambda (serverless) |
| **Framework** | Alexa Skills Kit (ASK) SDK for Python |
| **Speech Recognition** | Alexa Voice Service |
| **Audio Playback** | Alexa **AudioPlayer Interface** |
| **Interaction Model** | Custom Alexa Skill Model |
| **Deployment** | AWS Lambda, AWS CLI, or ASK CLI |

---

## 📡 Stream Information

The skill fetches the **live stream URL** from Kantipur Radio’s official online streaming service.

- **Streaming URL:** `https://example-stream-url.com`
- **Audio Format:** MP3 / AAC (adjusted based on device capability)
- **Bitrate:** Adaptive, depending on internet speed

---

## 🏗️ Project Structure

```plaintext
kantipur-radio-skill/
├── lambda/                      # AWS Lambda function directory
│   ├── lambda_function.py       # Main Alexa skill handler
│   ├── requirements.txt         # Python dependencies
│   └── languages/               # Multi-language support files
│       ├── en-US.json
│       ├── en-GB.json
│       ├── en-IN.json
│       ├── en-AU.json
│       └── en-CA.json
├── interactionModels/           # Alexa skill interaction models
│   └── custom/
│       ├── en-US.json
│       ├── en-GB.json
│       ├── en-IN.json
│       ├── en-AU.json
│       └── en-CA.json
├── assets/                      # Static assets
│   └── images/                  # Alexa skill icons
│       ├── en-US_smallIconUri.png
│       ├── en-US_largeIconUri.png
│       └── ... (other locale images)
├── skill.json                   # Alexa skill configuration file
├── LICENSE                      # Open-source MIT License
└── README.md                    # Project documentation
```

---

## 🚀 Deployment Guide

1. **Install Dependencies**  
   ```bash
   pip install -r lambda/requirements.txt
   ```

2. **Test Locally with ASK CLI**  
   ```bash
   ask dialog --locale en-US
   ```

3. **Deploy the Skill to AWS Lambda**  
   ```bash
   ask deploy
   ```

4. **Enable the Skill on Alexa Developer Console**
   - Go to **https://developer.amazon.com**
   - Upload `skill.json`
   - Configure the invocation name
   - Test in the Alexa Simulator

---

## 🔑 Requirements

To use the **Kantipur Radio Alexa Skill**, you need:
- An **Alexa-enabled device** (Amazon Echo, Echo Dot, Fire TV, etc.)
- A **stable internet connection**
- A device that **supports audio playback**

---

## 📜 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---

## 📢 Support

If you encounter any issues, say **"Alexa, help"** while using the skill for assistance.

For further inquiries, visit our **GitHub repository** or contact us.

---

## 📝 Notes

- This skill is designed for **simplicity and accessibility**.
- **Audio quality** depends on **internet speed and streaming availability**.
- Advanced features like **loop, shuffle, and track selection** are not supported since this is a **live radio stream**.

---

**Made with ❤️ for Nepali radio listeners worldwide!** 🎵🇳🇵
