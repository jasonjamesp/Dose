
Dose: Medication Tracker App

📖 About the Project

Dose is a native Android application designed to overcome digital accessibility barriers for the elderly population. Existing solutions often fail due to complex navigation or reliance on the internet. This project provides a straightforward, accessible solution that empowers elderly users to manage their health independently through simple and consistent notification mechanisms.
🎯 Project Objectives

    User-Friendly Design: To develop an intuitive user interface (UI) specifically optimized for elderly users with high-contrast elements and simple navigation.

    Reliable Scheduling: To enable reliable medication scheduling with customizable reminders that function without internet connectivity.

    Data Privacy: To ensure data privacy and integrity by storing all personal health information locally on the device using SQLite.

    Adherence Tracking: To provide a secure log for tracking dosage history (Taken/Skipped) to monitor long-term adherence.

    Timely Alerts: To implement a robust local notification system that ensures critical alerts are never missed.

⚙️ How It Works 

The system operates on a dedicated Android Architecture integrated with a Local Database to ensure reliability.

    Input: The user enters medication details (Name, Dosage, Time) via the simplified dashboard.

    Storage: Data is securely encrypted and stored in the local SQLite Database.

    Scheduling: The Android background service (AlarmManager) schedules precise notifications.

    Alert: A system-level alarm triggers at the scheduled time, waking the device if necessary.

    Action: The user acknowledges the dose as "Taken" or "Skipped."

    Logging: The system instantly updates the adherence log, creating a history record viewable by the user.

🛠️ Technical Stack

    Development Platform: Android Native (Java/Kotlin)

    IDE: Android Studio

    Architecture Pattern: MVVM (Model-View-ViewModel) for clean code separation.

    Local Database: SQLite (via Room Persistence Library) for secure, offline storage.

    User Interface: XML Layouts with Material Design components for accessibility.

    Core System Services:

        AlarmManager: For precise, reliable scheduling of reminders even when the app is killed.

        NotificationManager: To handle system-level alerts and priority channels.

        BroadcastReceiver: To listen for system events (like device reboot) to reschedule alarms.
