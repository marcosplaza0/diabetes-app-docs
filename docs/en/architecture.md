# 🧱 Application Architecture – Diabetes App

This document describes the technical architecture of the Diabetes Management App, including the main parts, tools, and design decisions used in the development.

---

## ⚙️ Technologies Used

- **Flutter** – UI framework for cross-platform development
- **Dart** – Main programming language
- **Local Storage** – (To be chosen: Hive, SQLite...)
- **Charting** – `fl_chart` or similar package for data visualization
- **Notifications** – `flutter_local_notifications` for reminders

---

## 🧭 App Architecture Overview

The app follows a **layered architecture**, with separation of responsibilities:

```plaintext
Presentation Layer (UI)
│
├── State Management (e.g., Provider)
├── Data Layer
│   ├── Local Storage (e.g., Hive)
│   └── Models (GlucoseEntry, Reminder, etc.)
```

---

## 📱 Screens & Navigation

*Note: Screens and views are different things.*

- **HomeScreen** – Daily summary plus quick log access
- **LogEntryScreen** – Form to add glucose or insulin
- **HistoryScreen** – Different ways for glucose trends and summary visualization
- **ChartScreen** – Graph view of glucose trends
- **ReminderScreen** – Manage reminders
- **SettingsScreen** – Language, theme, backup (future)

Navigation will use **`Navigator 2.0`** or a package like `go_router` for scalable routing.

---

## 🧩 Main Components

*Note: The components below are conceptual and may evolve as the app is developed.*
### 1. Models
- `GlucoseEntry`: stores value, date/time, notes
- `InsulinDose`: type, units, timestamp
- `Reminder`: type, time, repetition

### 2. Services
- `StorageService`: handles read/write to a database
- `NotificationService`: sets and cancels local reminders

### 3. Providers / Controllers
- Responsible for keeping track of app data in real time and making sure the UI updates properly when that data changes.

---

## 🧪 Testing Strategy

- Unit tests for model logic
- Widget tests for UI components
- Manual testing on Android/iOS devices

---

## 🔜 Future Considerations

- Add `CloudService` (e.g., Firebase) for sync
- Use encrypted storage for sensitive data