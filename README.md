<h1>NothingNews</h1> <br>
Raw. Monochrome. Information. <br>
A minimalist news aggregator designed specifically for the Nothing OS ecosystem. Built to strip away the noise of modern media and present headlines in a clean, battery-friendly monochrome interface. <br>
📱 The Concept <br>
Most news apps are cluttered, colorful, and distracting. Nothing News embraces the philosophy of "Technology that feels like nothing." <br>
Zero Distractions: No clickbait thumbnails, just text. <br>
OLED Friendly: Pure black background for maximum battery efficiency. <br>
Cohesive Design: Uses the signature Dot Matrix typography and Glyph interface language. <br>
⚡ Features <br>
🔴 Visual Identity: Custom CSS implementation of the Nothing design language. <br>
📰 Live Feed: Fetches latest tech and world headlines. <br>
🔧 Modern Engine: Built on Capacitor 7, targeting Android SDK 35. <br>
✨ Adaptive Icons: Custom monochrome launcher icon. <br>
👆 Reader Mode: Distraction-free article viewing with smooth animations . <br>
Website for Mac/Windows:https://n-newz.vercel.app/ <br>
📥 Download <br>
You can download the latest .apk from the <a href='https://github.com/CoderBhoid/NothingNews/releases/tag/releases'>releases</a>. <br>
Requirements: <br>
Android 6.0 or higher. <br>
Optimized for Nothing Phone (1), (2), and (2a). <br>
🛠️ Tech Stack <br>
Core: HTML5, CSS3, Vanilla JavaScript <br>
Bridge: Capacitor 7 (Latest) <br>
Build System: Gradle (Android SDK 35) <br>
Compatibility: Java 17 / OpenJDK 17 <br>
🏗️ How to Build (Development) <br>
This project uses a specific configuration to run Capacitor 7 using Java 17. If you want to build this from source, follow these steps exactly. <br>
1. Prerequisites <br>
Node.js installed. <br>
Android Studio (Ladybug or newer) with SDK 35 installed. <br>
Java 17 (set as JAVA_HOME) <br>
2. Setup <br>
# Clone the repo <br>
git clone [https://github.com/yourusername/nothing-news.git](https://github.com/yourusername/nothing-news.git) <br>
# Install dependencies <br>
npm install <br>
3. Sync & Build <br>
This project requires specific Gradle configurations to bypass the Java 21 requirement of Capacitor 7. <br> 
# Generate Android project folder <br>
npx cap add android <br>
# Sync web assets <br>
npx cap sync <br>
Note on Build Errors: <br>
If you encounter invalid source release: 21, ensure the android/build.gradle file contains the afterEvaluate block forcing <br> JavaVersion.VERSION_1_8 or 17. <br>
4. Generate APK <br>
cd android <br> 
./gradlew assembleDebug <br>
The APK will be located at android/app/build/outputs/apk/debug/. <br>
📄 License <br>
Distributed under the MIT License. See LICENSE for more information. <br>
"Whatever you do, keep it simple." <br>
"Proudly Opensource" <br>
