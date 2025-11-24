<h1>NothingNews</h1>
Raw. Monochrome. Information.
A minimalist news aggregator designed specifically for the Nothing OS ecosystem. Built to strip away the noise of modern media and present headlines in a clean, battery-friendly monochrome interface.
📱 The Concept
Most news apps are cluttered, colorful, and distracting. Nothing News embraces the philosophy of "Technology that feels like nothing."
Zero Distractions: No clickbait thumbnails, just text.
OLED Friendly: Pure black background for maximum battery efficiency.
Cohesive Design: Uses the signature Dot Matrix typography and Glyph interface language.
⚡ Features
🔴 Visual Identity: Custom CSS implementation of the Nothing design language.
📰 Live Feed: Fetches latest tech and world headlines.
🔧 Modern Engine: Built on Capacitor 7, targeting Android SDK 35.
✨ Adaptive Icons: Custom monochrome launcher icon.
👆 Reader Mode: Distraction-free article viewing with smooth animations.
Website for Mac/Windows:https://n-newz.vercel.app/
📥 Download
You can download the latest .apk from the [suspicious link removed].
Requirements:
Android 6.0 or higher.
Optimized for Nothing Phone (1), (2), and (2a).
🛠️ Tech Stack
Core: HTML5, CSS3, Vanilla JavaScript
Bridge: Capacitor 7 (Latest)
Build System: Gradle (Android SDK 35)
Compatibility: Java 17 / OpenJDK 17
🏗️ How to Build (Development)
This project uses a specific configuration to run Capacitor 7 using Java 17. If you want to build this from source, follow these steps exactly.
1. Prerequisites
Node.js installed.
Android Studio (Ladybug or newer) with SDK 35 installed.
Java 17 (set as JAVA_HOME)
2. Setup
# Clone the repo
git clone [https://github.com/yourusername/nothing-news.git](https://github.com/yourusername/nothing-news.git)
# Install dependencies
npm install
3. Sync & Build
This project requires specific Gradle configurations to bypass the Java 21 requirement of Capacitor 7.
# Generate Android project folder
npx cap add android
# Sync web assets
npx cap sync
Note on Build Errors:
If you encounter invalid source release: 21, ensure the android/build.gradle file contains the afterEvaluate block forcing JavaVersion.VERSION_1_8 or 17.
4. Generate APK
cd android
./gradlew assembleDebug
The APK will be located at android/app/build/outputs/apk/debug/.
📄 License
Distributed under the MIT License. See LICENSE for more information.
"Whatever you do, keep it simple."
"Proudly Opensource"
