# Smart With You Project

## 📋 Project Overview
Smart With You เป็นโครงการที่รวมเอา Frontend Mobile และ Backend Server เข้าด้วยกัน เพื่อให้บริการสมบูรณ์แบบ

---

## 🏗️ Project Structure

```
Smartwithyouproject/
├── finalproject/
│   ├── myflutterproject/        # Frontend Mobile Application (Flutter)
│   ├── backend-django/          # Backend Server (Django REST)
│   ├── admin_panel/             # Admin Dashboard
│   └── README.md
```

### 📱 Frontend - myflutterproject (Flutter)
- **Framework:** Flutter
- **Language:** Dart
- **Purpose:** Mobile application for end users

### 🔧 Backend - backend-django (Django)
- **Framework:** Django REST Framework
- **Language:** Python
- **Purpose:** RESTful API Server
- **Database:** MySQL / PostgreSQL
- **Containerization:** Docker

### 👨‍💼 Admin Panel - admin_panel
- Administrative dashboard for managing system

---

## 🛠️ Technologies Used

### Frontend (Flutter/Dart)
- **Core Framework:** Flutter (SDK: ^3.5.3)
- **State Management:** Provider (^6.1.2)
- **HTTP Client:** http (^1.2.2)
- **Local Storage:** shared_preferences (^2.0.15)
- **WebSocket:** web_socket_channel (^3.0.1)
- **Firebase:**
  - firebase_core (^2.17.0)
  - firebase_messaging (^14.0.5)
- **Notifications:** flutter_local_notifications (^18.0.1)
- **Maps:** 
  - google_maps_flutter (^2.10.0)
  - flutter_map (^5.0.0)
  - latlong2 (^0.9.1)
  - location (^5.0.3)
- **Google APIs:**
  - googleapis (^11.0.0)
  - googleapis_auth (^1.4.0)
  - flutter_web_auth (^0.6.0)
- **Media:**
  - image_picker (^1.1.2)
  - webview_flutter (^4.10.0)
- **Utilities:**
  - intl (^0.18.0)
  - url_launcher (^6.3.1)
  - add_2_calendar (^3.0.1)
  - permission_handler (^11.3.1)
  - google_fonts (^6.1.0)
  - lottie (^2.7.0)
  - flutter_foreground_task (^8.17.0)

### Backend (Django/Python)
- **Web Framework:** Django (5.1.4)
- **REST API:** Django REST Framework (3.15.2)
- **Authentication:** djangorestframework-simplejwt (5.3.1)
- **CORS:** django-cors-headers (4.6.0)
- **Async Support:**
  - channels (4.2.0)
  - daphne (4.1.2)
  - channels_redis (4.2.1)
- **Background Tasks:**
  - celery (5.4.0)
  - django-celery-beat (2.7.0)
  - redis (5.2.1)
- **Scheduled Tasks:**
  - django-cron (0.6.0)
  - cron-descriptor (1.4.5)
- **Databases:**
  - mysqlclient (2.2.6)
  - psycopg2 (PostgreSQL support)
  - PyMySQL (1.1.1)
- **Push Notifications:** pyfcm (2.0.7), firebase-admin (6.6.0)
- **Google Cloud:**
  - google-cloud-firestore (2.20.0)
  - google-cloud-storage (2.19.0)
  - google-api-python-client (2.159.0)
- **Image Processing:** Pillow (11.0.0)
- **Security:** PyJWT (2.10.1)
- **Server:** Gunicorn (via daphne for async support)
- **Utilities:**
  - requests (2.32.3)
  - python-dateutil (2.9.0.post0)
  - pytz (2025.1)

---

## ⚙️ Architecture

### Backend Architecture
```
Backend (Django)
├── REST API Endpoints
├── WebSocket Support (Channels)
├── Celery Background Tasks
├── Firebase Integration
├── Google Cloud Services
└── Database (MySQL/PostgreSQL)
```

### Frontend Architecture
```
Frontend (Flutter)
├── UI Screens (Material Design)
├── State Management (Provider)
├── API Communication (HTTP)
├── Real-time Updates (WebSocket)
├── Firebase Push Notifications
├── Maps & Location Services
└── Local Storage (SharedPreferences)
```

---

## 🚀 Key Features

### Real-time Communication
- WebSocket for live updates
- Push Notifications via Firebase
- Background task handling with Celery

### Location-based Services
- Google Maps integration
- Location tracking
- Map display and navigation

### Authentication & Authorization
- JWT Token-based authentication
- CORS support for cross-origin requests
- Permission handling on mobile

### Cloud Services
- Firebase Cloud Messaging
- Google Cloud Firestore
- Google Cloud Storage
- Google Calendar integration

### Media Handling
- Image upload and processing
- File management
- WebView support for embedded content

---

## 📦 Installation & Setup

### Backend Setup
```bash
# 1. Clone the repository
git clone https://github.com/BomNattawut/Smartwithyouproject.git

# 2. Navigate to backend directory
cd finalproject/backend-django

# 3. Create virtual environment and activate
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Configure environment variables
# (Add your Google Keys and Firebase config)

# 6. Run migrations
python manage.py makemigrations
python manage.py migrate

# 7. Start the server
cd backend
python manage.py runserver
```

### Frontend Setup
```bash
# 1. Navigate to flutter project
cd finalproject/myflutterproject

# 2. Get Flutter packages
flutter pub get

# 3. Configure Google Services
# (Add google-services.json or GoogleService-Info.plist)

# 4. Run the app
flutter run
```

---

## 🔌 External Services Required

- **Firebase:** Authentication, Messaging, Cloud Storage
- **Google APIs:** Maps, Calendar, Drive
- **Database:** MySQL or PostgreSQL
- **Redis:** For caching and Celery broker
- **Google Cloud:** Firestore, Storage

---

## 📝 Notes

- Project uses Docker for containerization of backend
- Supports both real-time and scheduled task processing
- Mobile-first approach with responsive Flutter UI
- Enterprise-grade security with JWT and CORS

---

## 👨‍💻 Development Guidelines

- Backend: RESTful API design with DRF
- Frontend: Flutter best practices with Provider pattern
- Real-time: WebSocket for live features
- Notifications: Firebase Cloud Messaging integration
- Maps: Google Maps for location services

---

**Last Updated:** 2026-06-12
