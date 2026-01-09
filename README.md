# Chat App

A Flutter chat application that uses Firebase for authentication, real-time messaging, media storage, and push notifications.

---

## Key Features ✨

- **Email/password authentication** with Firebase Auth
- **Realtime chat** using Cloud Firestore (messages ordered and grouped by user)
- **User profile images** stored in Firebase Storage
- **Push notifications** via Firebase Cloud Messaging (topic & device tokens)
- Image picking from device camera using `image_picker`
- Clean UI with message grouping and avatar display

---

## Tech Stack & Requirements 🔧

- Flutter SDK: **>= 3.7.2** (see `pubspec.yaml`)
- Dart SDK as required by Flutter SDK above
- Main dependencies:
  - `firebase_core`, `firebase_auth`, `cloud_firestore`, `firebase_storage`
  - `firebase_messaging`
  - `image_picker`
- Platforms: Android & iOS

---

## App Structure (high-level) 🔎

- `lib/main.dart` — app entry and auth state routing
- `lib/views/auth_screen.dart` — login/signup UI and Firebase auth flows
- `lib/views/chat_screen.dart` — main chat UI & FCM setup
- `lib/widgets/chat_messages.dart` — message stream and list rendering
- `lib/widgets/message_bubble.dart` — message UI with grouping
- `lib/widgets/new_message.dart` — message composer (text + image)
- `lib/widgets/user_image_picker.dart` — camera image picker

---

## 📦 Download APK

Want to try the app without building it?

👉 [Download the APK](https://drive.google.com/file/d/1_fS54ccchjUWLiFmeQdha95NfLmTH1K6/view?usp=share_link)

---

## Testing & Debugging 🧪

- Test authentication by signing up & logging in.
- Use Firestore console to monitor the `chat` collection.
- For push notifications, test topic messages from Firebase Console or send to device token.
- Use `flutter run --debug` to view runtime logs.

---

## 📱 Preview

| Auth Screen                                                                              | Chat Screen                                          |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| ![Home](assets/screenshots/auth_screen.png) ![Home](assets/screenshots/auth_screen2.png) | ![Entertainment](assets/screenshots/chat_screen.png) |
