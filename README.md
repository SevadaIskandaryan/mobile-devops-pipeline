# Mobile DevOps Pipeline

A complete demonstration repository for Android Mobile DevOps, including automated CI/CD, Fastlane build lanes, and deployment-ready pipelines.

## 🚀 What’s Included

- End-to-end Android build automation with Fastlane
- GitHub Actions CI workflow for pull requests and pushes
- Automatic debug APK generation and artifact upload
- Extensible Fastlane lanes for build, test, release, and beta
- Clear DevOps workflow for mobile teams

## 📁 Project Structure

```
mobile-devops-pipeline/
├─ android-app/
│  ├─ app/                # Android app module (Kotlin)
│  ├─ build.gradle.kts    # Root Gradle build config
│  ├─ fastlane/           # Fastlane lanes and config
│  └─ ...
├─ .github/
│  └─ workflows/
│     └─ android.yml      # GitHub Actions pipeline
└─ README.md
```

## 🧭 Getting Started

1. Clone this repo:

```bash
git clone https://github.com/SevadaIskandaryan/mobile-devops-pipeline.git
cd mobile-devops-pipeline/android-app
```

2. Install Fastlane (Ruby required):

```bash
gem install fastlane
```

3. Build debug APK:

```bash
fastlane build
```

4. Find the generated APK:

- `app/build/outputs/apk/debug/app-debug.apk`

## ⚙️ Fastlane Lanes

- `fastlane build` — Build debug APK
- `fastlane test` — Placeholder for tests (extendable)
- `fastlane release` — Placeholder for release automation
- `fastlane beta` — Placeholder for beta deployment

## 📦 CI/CD Behavior

The GitHub Actions workflow in `.github/workflows/android.yml`:
- Builds the app on each push and PR
- Runs Fastlane build lane
- Uploads APK artifact from `app/build/outputs/apk/debug/`

## 🧩 Tech Stack

- CI/CD: GitHub Actions
- Build Automation: Fastlane
- Android: Kotlin
- Build System: Gradle
- Version Control: Git

## 💡 Notes

This project is intentionally minimal and designed for learning and portfolio usage. You can quickly extend the Fastlane lanes and CI YAML to add real unit tests, lint checks, or deployment targets.

## 👤 Author
Sevada Iskandaryan

[GitHub](https://github.com/SevadaIskandaryan)
