# **Practical 7 — Mobile Application Development (MAD)**

## **Retrieve JSON Data From API & Store in SQLite Database (Android App)**

**Submitted By:** OM KUSHWAHA
**Enrollment No:** 24012022002

---

## 📌 **AIM**

**Develop an Android application that retrieves person data in JSON format from an internet API and stores the retrieved data in an SQLite database.**

---

## 📖 **Overview**

This Android application demonstrates how to fetch structured JSON data from an online REST API, parse the response in Kotlin, and store the retrieved records into an SQLite database. It showcases essential Android concepts including API integration, background threading, database operations, and dynamic UI updates.

---

## 🧠 **Learning Objectives**

* Understand how to consume JSON data from an API using Android networking libraries.
* Learn how to parse JSON objects and arrays using Kotlin.
* Implement an SQLite database for local data storage.
* Insert, update, retrieve, and display stored data using SQLite CRUD operations.
* Update UI dynamically after storing data.

---

## ⚙️ **Features Implemented**

### ✔ **1. API Fetching**

* The app makes an HTTP GET request to fetch person data (name, email, phone, etc.) in JSON format.
* Libraries used: `Retrofit` or `HttpURLConnection` (based on your project structure).

### ✔ **2. JSON Parsing**

* The JSON response is parsed into Kotlin data classes.

### ✔ **3. SQLite Database Integration**

* Uses `SQLiteOpenHelper` to create tables.
* Inserts fetched data into the local database.
* Retrieves stored data to display on screen.

### ✔ **4. UI Components**

* A button to fetch API data.
* A button or activity to show stored data.
* A RecyclerView/ListView to display person details.

---

## 🛠 **Technologies Used**

* **Language:** Kotlin
* **UI:** XML Layouts
* **Database:** SQLite (SQLiteOpenHelper)
* **JSON Parsing:** Kotlin Data Classes
* **Networking:** Retrofit / HttpURLConnection
* **IDE:** Android Studio
* **Architecture:** Activity + Helper Classes

---

## 🧩 **Application Flow**

1. User opens app → main screen loads.
2. User taps *Fetch Data* → app calls the API.
3. JSON data is received and parsed.
4. Parsed data is stored into the SQLite database.
5. User can navigate to *View Data* screen to see the stored records.

---

## 📂 **Repository Structure**

```
/app
   /src
      /main
         /java/yourpackage
             - MainActivity.kt
             - ApiService.kt
             - Person.kt (data class)
             - DBHelper.kt (SQLiteOpenHelper)
             - PersonAdapter.kt
         /res
             /layout
             /drawable
             /values
```

---

## ▶️ **How to Run the Project**

1. Clone or download the repository.
2. Open the project in **Android Studio**.
3. Let Gradle sync automatically.
4. Run the app on an emulator or physical Android device.
5. Press **Fetch Data** to retrieve JSON data.
6. Press **Show Data** to view saved SQLite entries.

---

## 🚀 **Future Enhancements**

* Add Room Database (modern SQLite wrapper).
* Add error handling for failed API calls.
* Add delete/update features for stored person data.
* Add loading animations during API fetch.
* Allow offline mode to view data without internet.

---

## ✔ **Conclusion**

This practical demonstrates how Android applications can integrate real-time internet APIs with local data storage, enabling offline capability and persistent data handling. It provides hands-on experience with networking, JSON parsing, and SQLite database operations using Kotlin.

---
