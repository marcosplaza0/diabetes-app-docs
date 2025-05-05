# 🧪 Testing Plan – Diabetes App

This document outlines the testing strategy for the Diabetes Management App. The goal is to ensure the app functions correctly, meets the requirements, and provides a stable user experience.

---

## ✅ Testing Goals

- Verify that core features work as expected
- Ensure data is stored and retrieved correctly
- Confirm that the UI responds properly to user actions
- Detect bugs early and prevent regressions
- Validate app behavior across different devices and platforms

---

## 🔍 Types of Testing

### 1. Manual Testing

Performed regularly during development using real devices and emulators.

#### Examples:
- Add a glucose reading → entry appears in the history
- Set a reminder → notification is triggered at the right time
- Delete an entry → entry is removed from the list
- Restart app → data is still available
- Change language in settings → UI updates correctly

---

### 2. Unit Testing

Focus on testing the logic of individual classes and functions, such as:

- GlucoseEntry model creation and validation
- Reminder scheduling logic
- Data calculations (e.g. averages, trends)

Tool: `flutter_test`

---

### 3. Widget Testing

Simulates user interaction with UI components.

Examples:
- Filling and submitting a form
- Pressing buttons (e.g. Save, Delete)
- Navigating between screens

Tool: `flutter_test`

---

### 4. Device/Platform Testing

Tests on both Android and iOS to ensure consistency and compatibility.

#### Devices:
- Android emulator (Google Pixel 8, API 30+)
- iOS emulator (iPhone 13)
- Physical Device: Xiaomi Redmi Note 12 pro plus 5G

---

## 🧩 Testing Tools

- `flutter_test`: built-in testing framework
- `integration_test`: for full app testing (optional in future)

---

## 📆 Testing Schedule

| Phase              | Type                | Status     |
|--------------------|---------------------|------------|
| During development | Manual & unit tests | To be done |
| Before MVP release | Full widget tests   | To be done |
| Final submission   | Manual + summary    | To be done |

---

## 📝 Notes

- All test results will be reviewed and documented before delivery.
- Bugs and UI inconsistencies will be logged in GitHub issues or project board.
