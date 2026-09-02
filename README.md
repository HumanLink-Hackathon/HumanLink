# HumanLink 🇬🇭

> **Connecting Every Voice Through Inclusive Technology.**

[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.x-0175C2?logo=dart)](https://dart.dev)
[![Hackathon](https://img.shields.io/badge/MTN%20Ghana-T%C9%9Bkyer%C9%9Bma%20Pa%20Hackathon%202026-yellow)](https://github.com/HumanLink-Hackathon/HumanLink)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

**HumanLink** is an inclusive communication platform designed to remove language and disability barriers across Ghana. By bridging Ghanaian languages (starting with **Twi**), English, real-time live captioning, and controlled Ghanaian Sign Language representations, HumanLink empowers Deaf and hard-of-hearing individuals, native language speakers, customer service agents, and educators to communicate seamlessly.

---

## 📖 Table of Contents

- [The Challenge & Vision](#-the-challenge--vision)
- [Core Communication Pipeline](#-core-communication-pipeline)
- [Key Features](#-key-features)
- [Architecture & Tech Stack](#-architecture--tech-stack)
- [Project Directory Structure](#-project-directory-structure)
- [Getting Started](#-getting-started)
- [Team & Collaboration](#-team--collaboration)
- [Roadmap](#-roadmap)
- [License](#-license)

---

## 🎯 The Challenge & Vision

In Ghana, millions communicate primarily in indigenous languages such as Twi, while many essential services (banking, telecommunications, government, healthcare, higher education) operate predominantly in English or via spoken audio. For the **Deaf and hard-of-hearing community**, this creates a double communication barrier.

> **HumanLink Product Principle:** *Technology should adapt to people, not force people to adapt to technology.*

Rather than a simple text translator, HumanLink serves as an **end-to-end communication bridge**:
* **Inclusive Customer Service**: Facilitating smooth communication between Deaf/Twi-speaking customers and MTN customer service representatives (e.g., Mobile Money guidance, SIM registration).
* **Educational Accessibility**: Real-time high-contrast lecture captioning for university and high school classrooms.
* **Financial Inclusion**: Clear, accessible visual and sign representations of financial and mobile money concepts.

---

## 🔄 Core Communication Pipeline

```text
                  HUMANLINK ENGINE
                         │
                         ▼
                   USER SPEAKS
                         │
                         ▼
             ┌───────────────────────┐
             │ SPEECH-TO-TEXT ENGINE │
             └───────────┬───────────┘
                         │
                         ▼
                  RECOGNIZED TEXT
                         │
                         ▼
              ┌─────────────────────┐
              │ LANGUAGE PROCESSOR  │
              │   (Twi ↔ English)   │
              └──────────┬──────────┘
                         │
                         ▼
             ┌───────────────────────┐
             │ MULTI-MODAL OUTPUT    │
             │        ENGINE         │
             └───────────┬───────────┘
                         │
         ┌───────────────┼───────────────┐
         ▼               ▼               ▼
   LIVE CAPTIONS    SIGN LANGUAGE   SPEECH (TTS)
  (High Contrast)    (Visual/GIF)     (Spoken)
```

---

## ✨ Key Features

1. 🎙️ **Speech Recognition**: Real-time audio capture and transcription in Twi and English.
2. 🔄 **Bidirectional Translation**: Accurate Twi ↔ English language processing.
3. 💬 **High-Contrast Live Captions**: Real-time adjustable caption stream designed for Deaf and hard-of-hearing readers.
4. 🤟 **Controlled Sign Language Output**: Rich visual cards and animations representing key phrases (Greetings, Help, Mobile Money, Balance, Transactions).
5. 📱 **MTN Financial & Customer Care Simulation**: Purpose-built accessible interface for MoMo balance checks, account assistance, and transaction confirmations.
6. ♿ **Accessibility-First Design**: Custom high-contrast theme, dynamic text scaling (Small, Medium, Large, XL), screen reader support, and haptic feedback.

---

## 🛠️ Architecture & Tech Stack

* **Mobile / Web Frontend**: Flutter 3.x & Dart 3.x
* **State Management**: Provider / Riverpod
* **Audio & Speech**: `speech_to_text`, `flutter_tts`, `record`
* **Local Storage & Cache**: `shared_preferences`
* **Accessibility UI**: Custom Accessibility Engine & High-Contrast Design System
* **CI/CD**: GitHub Actions

---

## 📂 Project Directory Structure

```text
humanlink/
├── .github/                  # Issue templates
├── assets/
│   ├── images/               # App illustrations & branding
│   ├── icons/                # Accessibility-focused UI icons
│   ├── signs/                # Curated sign language visuals
│   └── translations/         # Offline phrase dictionaries
├── docs/                     # Research, architecture & API specs
├── lib/
│   ├── ai/                   # Speech recognition & translation layer
│   │   ├── speech/
│   │   ├── translation/
│   │   └── sign_language/
│   ├── core/                 # Theme, accessibility engine, constants
│   │   ├── accessibility/
│   │   ├── constants/
│   │   ├── theme/
│   │   └── utils/
│   ├── features/             # Feature screens & controllers
│   │   ├── captions/
│   │   ├── conversation/
│   │   ├── financial_services/
│   │   ├── home/
│   │   └── sign_language/
│   ├── models/               # Domain data models
│   ├── services/             # Audio, TTS, API and storage services
│   ├── widgets/              # Reusable accessible UI components
│   └── main.dart             # Application entrypoint
└── test/                     # Unit and widget tests
```

---

## 🚀 Getting Started

### Prerequisites
* Flutter SDK (3.11+ recommended)
* Dart SDK
* Android Studio / VS Code with Flutter extension
* Git

### Installation & Run
```bash
# 1. Clone the repository
git clone https://github.com/HumanLink-Hackathon/HumanLink.git
cd HumanLink

# 2. Checkout develop branch
git checkout develop

# 3. Install dependencies
flutter pub get

# 4. Run the application
flutter run
```

---

## 👥 Team & Collaboration

Developed with ❤️ for the **MTN Ghana Tɛkyerɛma Pa Hackathon 2026** by **Team HumanLink**:

| Member | Role | GitHub |
| :--- | :--- | :--- |
| **Redeemer Jerrey Kow Williams** | Team Lead / Project & Technical Lead | [`@soarmedia`](https://github.com/soarmedia) |
| **Pearl Tulasi Mawufemo** | UI/UX & Accessibility | Pending |
| **Enock Kyei-Baffour** | Backend / AI Engineering | [`@Courteous05`](https://github.com/Courteous05) |
| **Hannah Aidoo** | Development & Research | [`@faculty-NA`](https://github.com/faculty-NA) |
| **Able Mwintuma Gambo** | Software Development & Testing | [`@mwintuma`](https://github.com/mwintuma) |

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for branch management, PR review guidelines, and coding standards.

---

## 🗺️ Roadmap

- [x] Project Foundation & Git Architecture
- [x] Accessibility Engine & Theme System
- [ ] Core Speech-to-Text & Twi Translation Engine
- [ ] Live Captioning Interface with Adjustable Typography
- [ ] Curated Ghanaian Sign Language Phrase Bank
- [ ] MTN Mobile Money Accessible Communication Simulator
- [ ] Integration Testing & Hackathon Demo Preparation

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.