
# 📬 Flutter Mail Client (IITK IMAP/SMTP)

A secure and user-friendly Flutter-based email client built for IIT Kanpur students and staff. This app connects to the IITK IMAP (`qasid.iitk.ac.in`) and SMTP (`mmtp.iitk.ac.in`) servers to provide core mail functionality like login, mail viewing, draft handling, and email composing.

---

## ✨ Features

- 🔐 **Secure Login** using `flutter_secure_storage`
- 📩 **Fetch Emails** via IMAP from IITK mail server
- ⭐ **Starred Messages** support with persistent state
- 📨 **Compose & Send Emails** using IITK SMTP
- 🧾 **Drafts** management and resume functionality
- 🔎 **Search** through emails by subject or sender
- 📥 **Load More Emails on Scroll**
- 🧵 HTML email rendering with `flutter_html` + table support

---

## 🛠 Tech Stack

- **Flutter** (Dart)
- **enough_mail** for IMAP/SMTP
- **flutter_secure_storage** for credential persistence
- **flutter_html** + **flutter_html_table** for rendering HTML emails

---

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (latest stable version)
- A valid IITK mail ID (`@iitk.ac.in`)

### Installation

```bash
git clone https://github.com/your-username/flutter-mail-client-iitk.git
cd flutter-mail-client-iitk
flutter pub get
flutter run
```

---

## 🔒 Security Notes

- Credentials are stored securely using Flutter Secure Storage.
- Make sure to handle logout properly to avoid leaving credentials behind.
- The app uses SSL connections for both IMAP and SMTP.

---

## 📂 Project Structure (Main Components)

| File | Description |
|------|-------------|
| `main.dart` | App entry point, login logic, and UI |
| `MessageListScreen` | Lists and manages fetched emails |
| `MessageDetailScreen` | Displays full email content |
| `MimeComposerScreen` | Composing and sending emails |
| `sendMimeMessageViaSmtp()` | SMTP email sending utility |

---

## ✅ To-Do (Improvements)

- Add support for attachments 📎
- Implement mail reply and forward
- Notification for new emails
- Theme customization (dark mode)

---

## 📧 Screenshots (Optional)

_Add screenshots of login, inbox, and mail detail screens here._

---

## 📄 License

MIT License

---

## 👤 Author

Developed as part of a student utility project for IIT Kanpur. Maintained by [Your Name].

---

## 📁 What's Inside the ZIP

This ZIP contains:
- A `README.md` file with full documentation
- Folder structure ready to be dropped into a GitHub repo or project directory

Use this as your project's landing page to help others understand and use your Flutter mail client.

---

## 🧑‍💻 How to Use the App

Here’s a step-by-step guide on how to use the Flutter Mail Client once it’s running:

### 1. **Login**
- Open the app.
- Enter your IITK email ID (must end with `@iitk.ac.in`).
- Enter your password and click **Login**.
- The app securely stores your credentials using `flutter_secure_storage`.

### 2. **View Inbox**
- Once logged in, your inbox will load with the latest 50 messages.
- Scroll down to automatically load older messages.

### 3. **Search**
- Use the search bar at the top to filter emails by **subject** or **sender**.

### 4. **Star Emails**
- Tap the ⭐ icon next to any email to mark it as important.
- Toggle the star filter to view only starred messages.

### 5. **Read Full Email**
- Tap on any email to view the full content.
- The app supports both plain text and HTML-rendered views.

### 6. **Compose Email**
- Click the ✏️ (edit) button to open the email composer.
- Fill in recipient, subject, body, and click send.
- Emails are sent using IITK’s SMTP server.

### 7. **Manage Drafts**
- You can save your composed emails as drafts.
- Access saved drafts using the 📄 (drafts) button.

### 8. **Logout**
- Click the logout icon in the top bar to safely exit the app.

---

This app is designed to make basic email access simple and mobile-friendly for IITK users.

