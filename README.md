# Therapy Companion

A Flutter-based mobile application designed to help users train positive cognitive responses to specific emotional triggers.

The app allows users to associate affirmations with personal triggers, reinforcing neural pathways through repetition and reflection. The goal is to help users build healthier mental responses over time.

The application runs entirely on-device using local storage, ensuring privacy and fast performance. The app is available to testers on the Play Store upon request.

The share feature allows users to export a CSV document containing trigger history and occurrence data to share with their therapists.

Soon, users will be able to vent to an AI model that provides a second opinion and behavioral insights. **NOT A MEDICAL DIAGNOSIS.**

---

## Screenshots

<img alt="1" src="https://github.com/user-attachments/assets/39f075f3-5a4b-499e-8efa-fe516236509e" width="250"/>
<img alt="2" src="https://github.com/user-attachments/assets/3dc013bb-d7a9-45ec-b8e2-02483601518b" width="250"/>

<img alt="4" src="https://github.com/user-attachments/assets/9f0c5fb0-e543-43e8-8713-705aee8bbb35" width="250"/>
<img alt="3" src="https://github.com/user-attachments/assets/cdbd2b93-c283-4af2-9f8f-f4ac29703019" width="250"/>

---

## Features

- **Trigger Tracking** – Record emotional triggers as they occur.
- **Affirmation Pairing** – Associate triggers with constructive cognitive responses.
- **Neural Reinforcement** – Encourages repeated interaction to strengthen positive mental associations.
- **History Timeline** – Review previously recorded triggers and responses.
- **Therapy Sharing Support** – Generate a shareable record of trigger history.
- **Local Storage** – All data remains on-device for privacy.
- **Minimal Mobile Interface** – Designed for fast, daily interaction.

---

## Technicals

### Core Tech Stack

#### Framework
- **Flutter & Dart**  
  Cross-platform development for Android, iOS, and Web (PWA).

#### Local Databases

**Relational (SQL)**
- **sqflite**  
  Manages relationships between:
  - Triggers
  - Episodes
  - Therapy notes

**NoSQL / Object Storage**
- **Hive**  
  High-performance storage for:
  - App state
  - User preferences
  - Cached configurations

#### Data Visualization
- **fl_chart**  
  Converts raw episode data into:
  - Trend graphs
  - Frequency heatmaps
  - Pattern insights

#### On-Device AI Engine
- **TensorFlow Lite (tflite_flutter)**  
  Powers the AI Second Opinion feature:
  - Fully on-device execution
  - CPU/GPU acceleration
  - No backend dependency

#### Utilities
- **intl** – Localization and date formatting  
- **share_plus** – Exporting summaries  
- **csv** – Data portability and backup  

---

### Special Data Structures

#### Relational Mapping
Custom schema linking **Triggers → Episodes**, enabling:
- Frequency analysis
- Correlation scoring
- Behavioral pattern detection

#### Chat Stream Model
Custom `ChatMessage` model that:
- Handles bidirectional dialogue
- Maintains conversational context
- Operates fully offline

#### JSON Serialization
Used to:
- Convert complex Dart objects
- Enable SQL storage compatibility
- Support CSV export

---

## Installation


1. Clone the repository:  
```bash
git clone https://github.com/sidsoftwareupload/therapy-companion-app.git
```

2. Navigate to project directory:
```bash
cd therapy-companion-app
```
3. Get dependencies:
```bash
flutter pub get
```
4. Run on device or emulator:
```bash
flutter run
```
