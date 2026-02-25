# 🚀 Complete Step-by-Step Tutorial

## Web vs Mobile Development + React Native Environment Setup (Windows)

This guide is designed for **Windows users** who want to set up a complete **React Native mobile development environment** and understand the core concepts behind it.

---

# 1️⃣ AI Overview – What Are We Building?

In modern development:

* 🌐 **Web Apps** → Run inside browsers
* 📱 **Mobile Apps** → Installed on Android/iOS devices

If you want to build cross-platform mobile apps using JavaScript, you use:

* **React** → For Web UI
* **React Native** → For Mobile Apps
* **Expo** → Simplified React Native development
* **Android Studio** → Android SDK + Emulator

---

# 2️⃣ Web vs Mobile Development (Concept Deep Dive)

## 🌐 Web Development

Runs in browser (Chrome, Edge, Firefox).

### Technologies:

* HTML
* CSS
* JavaScript
* Frameworks:

  * **React**
  * **Next.js**
  * **Angular**

### Advantages:

✔ Single codebase
✔ Cheap
✔ Instant updates

### Limitations:

❌ Limited device access
❌ Depends on browser performance

---

## 📱 Mobile Development

Installed apps on Android/iOS.

### Native Technologies:

* Android → Kotlin / Java
* iOS → Swift / Objective-C

### Cross-Platform:

* **React Native**
* **Flutter**

### Advantages:

✔ Better performance
✔ Full device access (camera, GPS, storage)
✔ Push notifications

### Limitations:

❌ App store approval
❌ Separate builds

---

# 3️⃣ React vs React Native

| Feature  | React            | React Native       |
| -------- | ---------------- | ------------------ |
| Platform | Web              | Mobile             |
| Tags     | `<div>`, `<img>` | `<View>`, `<Text>` |
| Output   | HTML             | Native components  |

**React Native uses React concepts but renders native mobile UI.**

---

# 4️⃣ Development Workflow Diagram

```
Your Code (JavaScript)
        ↓
React Native Framework
        ↓
Android SDK / iOS SDK
        ↓
Emulator / Real Device
        ↓
Mobile App Running
```

---

# 5️⃣ Software Installation (Windows – Step by Step)

---

# STEP 1️⃣ Install NVM (Node Version Manager)

### What is NVM?

**nvm manages Node.js versions.**

👉 You can switch between Node versions easily.

### Download:

Search: *nvm windows GitHub*

Install the Windows version.

After installation:

```
nvm list
```

Install Node 24:

```
nvm install 24.13.1
nvm use 24.13.1
```

Install LTS:

```
nvm install lts
```

Install specific version:

```
nvm install v18.20.8
```

Check versions:

```
node -v
npm -v
```

---

# STEP 2️⃣ Node.js & npm

### What is Node.js?

Node.js allows JavaScript to run outside the browser.

### What is npm?

npm = Node Package Manager

It:

* Installs libraries
* Manages dependencies
* Runs scripts

Example:

```
npm install react
```

---

# STEP 3️⃣ What is NPX?

**npx runs packages without installing globally.**

Example:

```
npx create-expo-app myApp
```

It downloads and runs temporarily.

---

# STEP 4️⃣ Install Android Studio

Download:

**Android Studio**

During installation:

✔ Install Android SDK
✔ Install Emulator
✔ Install Platform Tools

---

# STEP 5️⃣ Configure Android SDK

Open Android Studio:

```
More Actions → SDK Manager
```

Install:

* Android SDK Platform
* Android SDK Build Tools
* Android SDK Platform Tools
* Android Emulator
* Android NDK (optional but recommended)

---

# STEP 6️⃣ Create Virtual Device (Emulator)

```
Device Manager → Create Device
```

Recommended:

* Pixel 6
* RAM: 2GB+
* Storage: 8GB+

---

# STEP 7️⃣ Set Environment Variables (VERY IMPORTANT)

## 1️⃣ JAVA_HOME

Find JDK location inside Android Studio folder.

Set:

```
JAVA_HOME = C:\Program Files\Android\Android Studio\jbr
```

---

## 2️⃣ ANDROID_HOME

Usually:

```
C:\Users\YourName\AppData\Local\Android\Sdk
```

Set:

```
ANDROID_HOME = C:\Users\YourName\AppData\Local\Android\Sdk
```

---

## 3️⃣ Add to PATH

Add these paths:

```
%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\emulator
%ANDROID_HOME%\tools
%ANDROID_HOME%\tools\bin
```

Test:

```
adb --version
```

---

# 6️⃣ Expo vs React Native CLI

## 🔵 Expo

What is Expo?

**Expo Go**
App that runs your React Native project without full native build.

### Features:

✔ Fast setup
✔ Pre-built APIs
✔ Easy testing

Create project:

```
npx create-expo-app@latest myApp
cd myApp
npm run start
```

Scan QR with Expo Go.

---

## 🔴 React Native CLI

More control.

Create project:

```
npx react-native init MyApp
```

Run:

```
npm run android
```

Needs full Android setup.

---

# 7️⃣ Installation Architecture Diagram

```
Windows OS
   ↓
NVM
   ↓
Node.js
   ↓
npm / npx
   ↓
React Native / Expo
   ↓
Android Studio
   ↓
Android SDK
   ↓
Emulator
```

---

# 8️⃣ Git & GitHub (Basic Intro)

## Git

Version control system.

Commands:

```
git init
git add .
git commit -m "first commit"
```

## GitHub

Online hosting for Git repositories.

---

# 9️⃣ Choosing Platform Strategy

| Scenario             | Recommendation   |
| -------------------- | ---------------- |
| Startup MVP          | Web              |
| Daily Consumer App   | Mobile           |
| Cross Platform Fast  | Expo             |
| Large Production App | React Native CLI |

---

# 🔟 Final Learning Takeaways

You now understand:

✔ Web vs Mobile differences
✔ React vs React Native
✔ Node, npm, npx, nvm
✔ Expo vs React Native CLI
✔ Android Studio setup
✔ Environment variables
✔ Emulator setup
✔ Git basics

---

