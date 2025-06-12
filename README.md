# Flighter App

Flighter is a cross-platform mobile application for seamless flight booking, seat selection, payment processing, and real-time flight management. Built using **Flutter** (for the frontend) and **.NET** (for the backend), Flighter offers users an intuitive travel booking experience with secure transactions and dynamic features.

---

## 📁 Repository Structure

```
/src               → Contains all source code (Flutter + .NET)
/exe               → Contains pre-built executables or APKs
LiveDemoLinks      → Contains Published Links of Swagger and Dashboard
README.md          → Project overview and setup guide
```

---

## 📘 Project Overview

Flighter is a flight booking app designed to provide a fast, flexible, and secure way for travelers to book and manage flights.with BlazorWASM Dashboard, allowing real-time admin access to manage platform data. It includes features such as:

* Direct & round trip bookings
* Multi-currency support (EGP, USD)
* Intelligent chatbot assistant
* Offer-based deals
* Refund and payment policies
* Secure login and ticket management with downloadable PDFs
* Manageing Admins by Owner (Adding/removing Admins to/from specific Company)
* Managing Flights by Admins (Adding/removing Tickets,real time reveal for bookings and Users Over View)
*Real Time Reveal in Dashboard (Adding or deleting tickets/Admins doesn't require to refresh page)
Technologies used:

* **Flutter**: Frontend for mobile UI/UX
* **.NET Web API**: Backend APIs and services
* **Blazor WebAssembly**:  admin/owner dashboard 
---

## ⚙️ Setup Instructions

### 🖥️ System Requirements

| Component               | Version                       |
| ----------------------- | ----------------------------- |
| Flutter SDK             | >= 3.5.3                      |
| .NET SDK                | >= 8.0                        |
| Visual Studio	          | 2022 or later                 |
| SQL Server (optional)	  | 2019+ or LocalDB              |
| Android Studio/Xcode    | Latest stable                 |
| Visual Studio / VS Code | Latest stable                 |
| OS                      | Windows 10+ / macOS Monterey+ |

---

### 🚀 Option 1: Build from Source

#### 1. Clone the Repository

```bash
git clone https://github.com/Flighter-4u/flighter.git
cd flighter
```

### 🔧 Flutter (Frontend)

#### ✅ Prerequisites

* Flutter SDK: [https://flutter.dev/docs/get-started/install](https://flutter.dev/docs/get-started/install)
* Device/emulator setup
* Dart-enabled IDE (VS Code/Android Studio)
* At least one of the following device setups:

  * Chrome (for web)
  * Windows PC with Visual Studio (for Windows builds)
  * macOS with Xcode (for macOS builds)

#### 🧱 Compile & Run

```bash
cd src/Flighter
flutter pub get
flutter run
```
---

### 🧱 Compile & Run the App

```bash
cd src/Flighter
flutter pub get
flutter run
```

> ℹ️ Use `flutter devices` to list all available platforms on your system.

---

## 🖥️ Platform-Specific Instructions

### 🌐 Web

To run in the browser:

```bash
flutter run -d chrome
```

To build a static web app for deployment:

```bash
flutter build web
```

Output will be in: `build/web/`

---

### 🪟 Windows

> ⚠️ Requires [Visual Studio](https://visualstudio.microsoft.com/) with the **“Desktop development with C++”** workload.

To build the Windows executable:

```bash
flutter build windows
```

Then navigate to:

```
build/windows/runner/Release/
```

Launch the app by double-clicking:

```
Flighter.exe
```

---

### 🍎 macOS

> ⚠️ Requires a macOS system with [Xcode](https://developer.apple.com/xcode/) installed.

To build the macOS app:

```bash
flutter build macos
```

Then go to:

```
build/macos/Build/Products/Release/
```

Launch the app:

```
Flighter.app
```

---
You can contact us at flighter4u@gmail.com to request the source code.
---

### 🌐 .NET (Backend)

#### ✅ Prerequisites

* .NET SDK: [https://dotnet.microsoft.com/download/dotnet/8.0](https://dotnet.microsoft.com/download/dotnet/8.0)
* SQL Server (if needed)
* Update the connection string in appsettings.json if required

#### 🧱 Compile & Run

```bash
cd src/Src Flighter(.Net)
dotnet restore
dotnet build
dotnet run
```

---

### 📦 Option 2: Pre-built Executables

#### 📱 Android APK

1. Navigate to `/exe/Flighter apk/`
2. Install `app-release.apk` on your Android device
3. Enable installation from unknown sources if required

#### 🖥️ Web/Desktop (Optional)

1. Open the `/exe/` folder
2. Launch the corresponding file:

   * Windows: `Flighter.exe`
   * macOS: `Flighter.app`

🌐 Swagger (API Documentation)

1.You can run the API from the /exe/ folder by launching Flighter.Api.exe.
2.Once running, open your browser and navigate to:
  http://localhost:PORT/swagger
  Replace PORT with the actual port shown in the terminal (e.g., 5000, 7000).
  Or, access the hosted version 

---

## ⚙️ Configuration
For App:
* API Base URL in `lib/constants.dart` or `.env`
* Set Stripe keys and backend URIs as needed
For Backend:
* Make sure to review/update the settings in appsettings.json(ConnectionStrings,JwtSettings,SMTP)
* If your Blazor project makes HTTP requests to the API, the base URL must be set in one of the following:
  Program.cs or HttpClient registration
  Or a shared appsettings.json or .env-like config (if used)
---

## 🧯 Troubleshooting Tips

| Issue                   | Solution                                                    |
| ----------------------- | ----------------------------------------------------------- |
| `flutter pub get` fails | Check Flutter SDK installation                              |
| Emulator not starting   | Verify Android SDK setup                                    |
| .dll not found          | Install correct .NET Runtime                                |
| Database error          | Update it in appsettings.json                               |
|CORS error (for Blazor)  | Backend not allowing origin	Add frontend URL to CORS config |


---

For additional support, feel free to reach out or check the GitHub Issues page.

---

Made with ❤️ using Flutter & .NET

---
# Flighter Docs : https://flighters-organization.gitbook.io/flighter-docs

# Flighter Demo : https://drive.google.com/file/d/1yge8X3zWFqXF5p32XtbB7me12xB6NOZA/view?usp=drivesdk

## 🚀 Live Demos

- [📖 API Swagger UI](http://hmy.runasp.net/swagger/index.html)
- [🖥️ Blazor Dashboard](http://flighter-dashboard.runasp.net/login)

> More details : [`LiveDemoLinks.md`]

