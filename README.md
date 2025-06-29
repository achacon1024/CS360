Weight Tracking App
An Android application built in Java that allows users to log their daily weight, set goals, and receive motivational SMS alerts upon hitting milestones. Designed with simplicity, security, and user engagement in mind.

Features
User Authentication – Secure registration and login system using SQLite

Daily Weight Tracking – Log daily entries with visualized historical data

Goal Management – Set and track target weights with achievement notifications

Data Management – Full CRUD (Create, Read, Update, Delete) operations

SMS Notifications – Optional goal achievement alerts with proper permission handling

RecyclerView Display – Clean grid layout showing weight history by date

Technical Specifications
Platform: Android (Java)

Minimum SDK: API 21 (Android 5.0)

Target SDK: API 34 (Android 14)

Database: SQLite with normalized relational schema

Architecture: Modular, activity-based structure with separation of concerns

Permissions: Optional SEND_SMS with graceful degradation if denied

Installation
Clone the repository

Open in Android Studio

Build and run on a compatible Android device or emulator

Project Reflection
Meeting User Needs
The app was designed for users looking for a straightforward way to monitor their weight without the complexity of full-scale fitness apps. It delivers core functionality like secure data storage, daily logging, progress tracking, and simple goal management—features that promote accountability and help users stay consistent in their health goals.

UI Design and Screen Architecture
The UI is built around five key screens: login/registration, weight history, add-entry form, goal setting, and SMS preferences. Each screen is designed for a specific task and follows Material Design guidelines to ensure consistency and ease of use. Typography, color schemes, and layouts were carefully chosen to minimize cognitive load and enable users to complete actions in just a few taps.

Development Strategy
The project followed a modular, layered architecture. A DatabaseHelper class handled all database operations, while each Activity managed a focused part of the UI. The development process started with core features and gradually expanded, allowing for better testing and stability at each stage. Emphasis was placed on clean code, input validation, and error handling, especially around optional features like SMS.

Testing and Validation
Every major feature was tested manually, including edge cases and user interaction scenarios. Authentication was tested with invalid and valid inputs, database consistency was verified across sessions, and SMS permissions were tested with both allowed and denied states. Testing revealed the importance of clear user feedback and the value of fallback experiences when permissions are not granted.

Innovation and Challenges
A standout aspect of the project was implementing SMS notifications with graceful degradation. The challenge was offering a valuable feature (motivational texts) while still preserving full functionality if users declined the permission. This was solved with contextual permission requests, fallback UI-based celebrations, and clear communication around how and why the feature works.

Technical Proficiency
The SQLite database demonstrates solid relational design with enforced constraints and secure queries. The app also showcases advanced Android UI practices via RecyclerView, custom adapters, and responsive layouts. Permission handling was carefully crafted to comply with Android security standards and user privacy expectations. Overall, the app reflects full-stack Android development competence across database, UI, logic, and security layers.

License
This project was developed as part of a Mobile Application Development course. You’re welcome to use it for educational or reference purposes.

