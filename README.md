# 📱 QuoteBox

> A simple, elegant Android app that lets you save, view, and manage your favorite quotes — built with **Java**, **Android Studio**, and **SQLite**.

---

## 🌟 Features

- ✨ Beautiful splash screen on launch  
- 📝 Add and view personal quotes  
- 💾 Local storage using SQLite (no internet required)  
- 🗂️ Organized database via `DBHelper.java`  
- 🧩 Clean UI layouts (XML) for easy navigation  
- 🧪 Includes unit and instrumentation test templates  

---

## 🏗️ Tech Stack

| Component | Technology |
|------------|-------------|
| **Language** | Java |
| **IDE** | Android Studio (Gradle Kotlin DSL) |
| **Database** | SQLite (via `SQLiteOpenHelper`) |
| **UI Design** | XML Layouts |
| **Testing** | JUnit, Android Instrumentation |

---

## 📁 Project Structure

```text
quote_move/
├── app/
│   ├── src/main/java/com/example/quote_move/
│   │   ├── MainActivity.java
│   │   ├── AddQuoteActivity.java
│   │   ├── SplashActivity.java
│   │   └── DBHelper.java
│   ├── src/main/res/
│   │   ├── layout/
│   │   ├── values/
│   │   └── drawable/
│   ├── AndroidManifest.xml
│   └── build.gradle.kts
├── gradle/
├── settings.gradle.kts
└── gradle.properties

```
💡 How It Works

SplashActivity.java → Displays the splash screen when the app launches.
Navigates automatically to the main screen after a short delay.
MainActivity.java → Shows all saved quotes from the SQLite database.
Contains buttons to add, edit, or delete quotes.
AddQuoteActivity.java → Lets users add new quotes and authors.
On submission, it stores the data in the database using DBHelper.
DBHelper.java → Manages all database operations (create, insert, fetch, update, delete).
Uses SQLiteOpenHelper for local storage.
activity_main.xml, activity_add_quote.xml, activity_splash.xml →
Define the layout and interface of each screen.
res/values/ → Contains app configuration files like colors.xml, strings.xml, and themes.xml.
AndroidManifest.xml → Declares all app components, permissions, and the launcher activity.
