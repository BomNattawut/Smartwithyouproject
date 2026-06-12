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
| Library | Version | Purpose |
|---------|---------|---------|
| **flutter** | SDK | Core Framework |
| **intl** | ^0.18.0 | Internationalization |
| **cupertino_icons** | ^1.0.8 | iOS Style Icons |
| **http** | ^1.2.2 | HTTP Client |
| **shared_preferences** | ^2.0.15 | Local Storage |
| **provider** | ^6.1.2 | State Management |
| **web_socket_channel** | ^3.0.1 | WebSocket Communication |
| **firebase_core** | ^2.17.0 | Firebase Core |
| **firebase_messaging** | ^14.0.5 | Push Notifications |
| **flutter_local_notifications** | ^18.0.1 | Local Notifications |
| **permission_handler** | ^11.3.1 | Permission Management |
| **add_2_calendar** | ^3.0.1 | Calendar Integration |
| **url_launcher** | ^6.3.1 | URL Launcher |
| **googleapis** | ^11.0.0 | Google APIs |
| **googleapis_auth** | ^1.4.0 | Google Authentication |
| **flutter_web_auth** | ^0.6.0 | Web Auth Flow |
| **webview_flutter** | ^4.10.0 | WebView Support |
| **webview_flutter_android** | ^4.3.1 | Android WebView |
| **webview_flutter_wkwebview** | ^3.18.0 | iOS WebView |
| **flutter_map** | ^5.0.0 | Map Display |
| **latlong2** | ^0.9.1 | Location Coordinates |
| **image_picker** | ^1.1.2 | Image Selection |
| **google_maps_flutter** | ^2.10.0 | Google Maps |
| **location** | ^5.0.3 | Location Services |
| **flutter_foreground_task** | ^8.17.0 | Foreground Tasks |
| **google_fonts** | ^6.1.0 | Google Fonts |
| **lottie** | ^2.7.0 | Animations |

### Backend (Django/Python)

#### Core Framework & REST API
| Library | Version | Purpose |
|---------|---------|---------|
| **Django** | 5.1.4 | Web Framework |
| **djangorestframework** | 3.15.2 | REST API Framework |
| **djangorestframework-simplejwt** | 5.3.1 | JWT Authentication |
| **django-cors-headers** | 4.6.0 | CORS Support |

#### Real-time & Async Communication
| Library | Version | Purpose |
|---------|---------|---------|
| **channels** | 4.2.0 | WebSocket Support |
| **daphne** | 4.1.2 | ASGI Server |
| **channels_redis** | 4.2.1 | Redis Backend for Channels |
| **redis** | 5.2.1 | Redis Client |

#### Background Tasks & Scheduling
| Library | Version | Purpose |
|---------|---------|---------|
| **celery** | 5.4.0 | Async Task Queue |
| **django-celery-beat** | 2.7.0 | Celery Beat Scheduler |
| **django-cron** | 0.6.0 | Cron Tasks |
| **cron-descriptor** | 1.4.5 | Cron Description |

#### Database Drivers
| Library | Version | Purpose |
|---------|---------|---------|
| **mysqlclient** | 2.2.6 | MySQL Support |
| **psycopg2** | Latest | PostgreSQL Support |
| **PyMySQL** | 1.1.1 | MySQL Connector |

#### Cloud Services & APIs
| Library | Version | Purpose |
|---------|---------|---------|
| **firebase-admin** | 6.6.0 | Firebase Admin SDK |
| **google-cloud-firestore** | 2.20.0 | Firestore Database |
| **google-cloud-storage** | 2.19.0 | Cloud Storage |
| **google-api-python-client** | 2.159.0 | Google APIs |
| **google-auth** | 2.37.0 | Google Authentication |
| **google-auth-httplib2** | 0.2.0 | Google Auth HTTP |
| **google-auth-oauthlib** | 1.2.1 | Google OAuth |
| **google-cloud-core** | 2.4.1 | Google Cloud Core |
| **googleapis-common-protos** | 1.66.0 | Google Common Protos |

#### Image & Media Processing
| Library | Version | Purpose |
|---------|---------|---------|
| **Pillow** | 11.0.0 | Image Processing |
| **pyfcm** | 2.0.7 | FCM Push Notifications |

#### Security & Cryptography
| Library | Version | Purpose |
|---------|---------|---------|
| **PyJWT** | 2.10.1 | JWT Token Handling |
| **cryptography** | 44.0.0 | Cryptographic Functions |
| **pyOpenSSL** | 25.0.0 | OpenSSL Wrapper |

#### Date & Time
| Library | Version | Purpose |
|---------|---------|---------|
| **python-dateutil** | 2.9.0.post0 | Date Utilities |
| **pytz** | 2025.1 | Timezone Support |
| **django-timezone-field** | 7.1 | Django Timezone Field |

#### Async & Networking
| Library | Version | Purpose |
|---------|---------|---------|
| **aiohttp** | 3.11.11 | Async HTTP Client |
| **requests** | 2.32.3 | HTTP Client |
| **httplib2** | 0.22.0 | HTTP Library |
| **urllib3** | 2.3.0 | HTTP Utility |

#### Serialization & Data
| Library | Version | Purpose |
|---------|---------|---------|
| **msgpack** | 1.1.0 | Message Serialization |
| **protobuf** | 5.29.3 | Protocol Buffers |
| **sqlparse** | 0.5.3 | SQL Parser |

#### Server & Performance
| Library | Version | Purpose |
|---------|---------|---------|
| **gunicorn** | - | WSGI Server |
| **Twisted** | 24.11.0 | Async Networking |
| **whitenoise** | 6.9.0 | Static Files |

#### Utilities & Dependencies
| Library | Version | Purpose |
|---------|---------|---------|
| **attrs** | 24.3.0 | Class Utilities |
| **certifi** | 2024.12.14 | SSL Certificates |
| **click** | 8.1.8 | CLI Creation |
| **kombu** | 5.4.2 | Messaging Library |
| **vine** | 5.1.0 | Async Utils |

---

## ⚙️ Architecture

### Backend Architecture
```
Backend (Django)
├── REST API Endpoints
├── WebSocket Support (Channels + Redis)
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
- WebSocket for live updates (Channels + Redis)
- Push Notifications via Firebase & FCM
- Background task handling with Celery

### Location-based Services
- Google Maps integration
- Location tracking and services
- Map display and navigation

### Authentication & Authorization
- JWT Token-based authentication
- CORS support for cross-origin requests
- Google OAuth integration
- Permission handling on mobile

### Cloud Services
- Firebase Cloud Messaging
- Google Cloud Firestore
- Google Cloud Storage
- Google Calendar integration
- Firebase Admin SDK

### Media Handling
- Image upload and processing (Pillow)
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

- **Firebase:** Authentication, Messaging, Cloud Storage, Firestore
- **Google APIs:** Maps, Calendar, Drive, Cloud APIs
- **Database:** MySQL or PostgreSQL
- **Redis:** For caching and Celery broker
- **Google Cloud:** Firestore, Storage, Service Accounts

---

## 📝 Notes

- Project uses Docker for containerization of backend
- Supports both real-time (WebSocket) and scheduled task processing (Celery)
- Mobile-first approach with responsive Flutter UI
- Enterprise-grade security with JWT, OAuth, and SSL/TLS
- Async support with Daphne ASGI server

---

## 👨‍💻 Development Guidelines

- **Backend:** RESTful API design with DRF, async with Channels
- **Frontend:** Flutter best practices with Provider pattern
- **Real-time:** WebSocket with Redis backend for scalability
- **Notifications:** Firebase Cloud Messaging & FCM
- **Maps:** Google Maps for location services
- **Security:** JWT tokens, CORS validation, OAuth 2.0

---

**Last Updated:** 2026-06-12
**Dart SDK:** ^3.5.3
**Python:** 3.8+
