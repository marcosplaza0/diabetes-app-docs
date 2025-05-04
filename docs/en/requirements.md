# 📄 Project Requirements – Diabetes App

This document defines the functional and non-functional requirements for the *Diabetes Management App*, developed as a final-year project for the Multiplatform App Development course.

---

## ✅ 1. Functional Requirements

These are the core features the app must provide to fulfill its purpose.

- **FR1**: The user can log blood glucose readings, including date, time, and value.
- **FR2**: The user can log insulin doses with amount and timestamp.
- **FR3**: The user can add notes for each entry (e.g., meals, activity, symptoms).
- **FR4**: The app displays past readings in a list with filters (e.g., day, week, range).
- **FR5**: The app shows charts/graphs of glucose trends over time.
- **FR6**: The user can set up reminders for:
    - Insulin injections
    - Glucose measurement
    - Medical appointments
- **FR7**: All user data is stored locally and persists even after closing the app.
- **FR8**: Users can edit or delete logged entries.

---

## 📋 2. Non-Functional Requirements

These define how the app should perform and behave.

- **NFR1**: The app must work **offline** without requiring internet access.
- **NFR2**: The app must preserve all user data after closing or restarting the app.
- **NFR3**: The app must work on both **Android and iOS** platforms.
- **NFR4**: The app must be developed using **Flutter** and **Dart**.
- **NFR5**: The user interface must follow **Material Design** guidelines.
- **NFR6**: The app language must be **Spanish**, with optional English support.
- **NFR7**: The app should follow accessibility best practices (e.g., readable fonts, contrast...).

---

## 📎 3. Constraints

- **Technology Constraint**: The app must be developed using the Flutter framework.
- **Time Constraint**: The first release of the project must be completed and submitted by the academic deadline.
- **Platform Constraint**: Only mobile platforms (Android/iOS) are supported in this version.

---

## 🚀 4. Future Considerations

Potential features to be added after the MVP release:

- **Export to PDF/CSV**: for sharing glucose logs with doctors or storing records.
- **Cloud backup & sync**: using Firebase or similar service.
- **Dark mode**: optional dark-themed or light-themed interface.