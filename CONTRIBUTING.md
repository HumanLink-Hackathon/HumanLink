# Contributing to HumanLink 🤝

Thank you for contributing to **HumanLink** for the **MTN Ghana Tɛkyerɛma Pa Hackathon 2026**!

## 🚀 Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/HumanLink-Hackathon/HumanLink.git
   cd HumanLink
   ```

2. **Install Flutter Dependencies:**
   ```bash
   flutter pub get
   ```

3. **Verify Environment:**
   ```bash
   flutter doctor
   ```

---

## 🌿 Git Branching Strategy

To keep collaboration clean and avoid merge conflicts:

* `main` — **Production / Demo Ready**. Only stable, tested features.
* `develop` — **Integration Branch**. Completed features are merged here first.
* Feature branches — Create your branch from `develop`:
  * `feature/speech-recognition`
  * `feature/twi-translation`
  * `feature/live-captions`
  * `feature/sign-language-library`
  * `feature/accessibility-theme`
  * `feature/financial-services-demo`
  * `fix/microphone-permission`

---

## 🛠️ Step-by-Step Workflow

1. Create and switch to your feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
2. Make your changes and test locally:
   ```bash
   flutter analyze
   flutter test
   ```
3. Commit your changes using conventional commit messages:
   ```bash
   git commit -m "feat: add real-time caption sizing controls"
   ```
4. Push your branch to GitHub:
   ```bash
   git push -u origin feature/your-feature-name
   ```
5. Open a **Pull Request (PR)** against `develop` (or `main`) on GitHub:
   [https://github.com/HumanLink-Hackathon/HumanLink/pulls](https://github.com/HumanLink-Hackathon/HumanLink/pulls)
6. Tag a team member for code review.

---

## 👥 Core Team Members & Roles

| Member | Role | GitHub |
| :--- | :--- | :--- |
| **Redeemer Jerrey Kow Williams** | Project & Technical Lead | [`@soarmedia`](https://github.com/soarmedia) |
| **Pearl Tulasi Mawufemo** | UI/UX & Accessibility | Pending |
| **Enock Kyei-Baffour** | Backend / AI Engineering | [`@Courteous05`](https://github.com/Courteous05) |
| **Hannah Aidoo** | Development & Research | [`@faculty-NA`](https://github.com/faculty-NA) |
| **Able Mwintuma Gambo** | Software Development & Testing | [`@mwintuma`](https://github.com/mwintuma) |

---

## 🔒 Security Best Practices

* **Never commit secrets**: No `.env`, `google-services.json`, or API keys in git.
* Keep all sensitive variables in a local `.env` file (which is git-ignored).
