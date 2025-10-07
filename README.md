# Smart India Hackathon Workshop
# Date: 07.10.25
## Register Number: 212224230096
## Name: Iniya E
## Problem Title 
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations
## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea
A “Smart Indoor Navigation and Assistance System” for railway stations that:

Uses indoor maps, QR/NFC markers, and Bluetooth beacons for real-time location tracking.

Provides turn-by-turn navigation inside stations.

Supports voice assistance (in multiple Indian languages).

Integrates with Indian Railways data to show live platform/train information.

Offers AR (Augmented Reality) view for easier guidance.

Includes accessibility support for the visually or physically impaired.

## Proposed Solution / Architecture Diagram
Mobile App / Web App

User interface to search facilities and navigate.

Displays real-time train and platform information.

Indoor Positioning System

Uses Bluetooth Low Energy (BLE) Beacons, Wi-Fi triangulation, or QR markers for indoor location tracking.

Backend Server

Stores station maps, facility coordinates, and user requests.

Fetches real-time data from Indian Railways APIs.

Database

Contains metadata of all facilities, coordinates, and accessibility features.

Admin Dashboard

For railway authorities to update facilities, maps, and announcements.

AI/ML Layer (optional)

For route optimization (e.g., least crowded route, shortest path).

<img width="1024" height="1024" alt="Gemini_Generated_Image_oubqk4oubqk4oubq" src="https://github.com/user-attachments/assets/0683e353-6a11-4ab1-8b07-41d54e38d35f" />


## Use Cases
Layer	Technology
Frontend (App)	Flutter / React Native / Android Studio (Kotlin)
Backend	Node.js / Express / Django / Flask
Database	MongoDB / PostgreSQL / Firebase
Positioning System	BLE Beacons / Wi-Fi triangulation / QR code scanning
Mapping	Google Maps SDK / Mapbox / OpenStreetMap
AI Layer (optional)	TensorFlow / Scikit-learn for route optimization
Voice Assistant	Google Speech API / AWS Polly / IndicTTS
Integration	Indian Railways API for real-time train & platform data

## Technology Stack
| Layer                                  | Component                          | Technologies / Tools                                                                                                                                                        | Purpose                                                                                     |
| -------------------------------------- | ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| **1. Frontend (User Interface)**       | **Mobile / Web Application**       | - **Flutter** (cross-platform)  <br> - **React Native** (alternative)  <br> - **Android Studio (Kotlin)** (if native Android)  <br> - **HTML, CSS, JS** (for web dashboard) | Provides user interface for passengers to navigate, search facilities, and view train info. |
| **2. Mapping & Navigation**            | **Indoor & Outdoor Mapping**       | - **Mapbox SDK** / **Google Maps SDK**  <br> - **OpenStreetMap** (open-source)  <br> - **ARCore / ARKit** (for AR navigation)                                               | Displays interactive indoor maps and turn-by-turn directions.                               |
| **3. Indoor Positioning System (IPS)** | **Location Tracking**              | - **Bluetooth Low Energy (BLE) Beacons**  <br> - **Wi-Fi Triangulation**  <br> - **QR Code Scanning** (for checkpoints)                                                     | Detects user’s location inside the station where GPS doesn’t work.                          |
| **4. Backend Server**                  | **APIs and Logic Processing**      | - **Node.js + Express.js** / **Django (Python)**  <br> - **Flask** (lightweight option)                                                                                     | Handles user requests, routes, and connects to databases & APIs.                            |
| **5. Database**                        | **Data Storage**                   | - **MongoDB** (NoSQL)  <br> - **PostgreSQL / MySQL** (SQL alternative)  <br> - **Firebase Firestore** (for real-time data)                                                  | Stores station maps, facility locations, user history, and preferences.                     |
| **6. Cloud & Hosting**                 | **Deployment**                     | - **AWS / Google Cloud / Azure**  <br> - **Firebase Hosting** (for smaller projects)                                                                                        | Hosts the backend, database, and API services.                                              |
| **7. Integration APIs**                | **External Data Sources**          | - **Indian Railways Live Train API**  <br> - **Railway Enquiry API (IRCTC / RapidAPI)**  <br> - **Google Places API**                                                       | Fetches real-time train info, schedules, and platform updates.                              |
| **8. Voice & Accessibility**           | **Speech and Accessibility Tools** | - **Google Speech-to-Text**  <br> - **Text-to-Speech (TTS) APIs** (Google, AWS Polly, IndicTTS)  <br> - **Language Translation API**                                        | Enables multilingual voice navigation and accessibility for visually impaired users.        |
| **9. AI / ML Layer (Optional)**        | **Smart Recommendations**          | - **Python (Scikit-learn / TensorFlow)**  <br> - **ML Models for Route Optimization**                                                                                       | Suggests best routes based on crowd density or accessibility needs.                         |
| **10. Admin Dashboard**                | **Management Panel**               | - **React.js / Angular / Vue.js**  <br> - **Bootstrap / Tailwind CSS**                                                                                                      | Used by station authorities to manage facility data and push alerts.                        |
| **11. Security & Authentication**      | **User Safety & Privacy**          | - **JWT (JSON Web Tokens)**  <br> - **OAuth 2.0 / Firebase Auth**                                                                                                           | Provides secure login and data access.                                                      |
| **12. Analytics & Monitoring**         | **Performance & Usage Tracking**   | - **Google Analytics**  <br> - **Grafana / Prometheus**                                                                                                                     | Tracks app performance, station usage, and navigation patterns.                             |


## Dependencies

1.Frontend (Flutter)

http – API calls

mapbox_gl – Map & navigation

geolocator – Location access

flutter_blue_plus – BLE beacon tracking

qr_code_scanner – QR marker scanning

flutter_tts / speech_to_text – Voice support

provider – State management

2.Backend (Node.js + Express)

express – API framework

mongoose – MongoDB connection

dotenv – Environment variables

cors – Cross-origin requests

jsonwebtoken, bcryptjs – Authentication

axios – External API calls

helmet – Security

nodemon – Development reload

3.Database

MongoDB Atlas – Cloud database

mongoose – ODM tool

4.Mapping & APIs

Mapbox SDK – Indoor navigation

Indian Railways API – Live train data

5. Voice & Accessibility

flutter_tts, speech_to_text

Google Speech API / Translate API

6.Cloud & Hosting

Firebase / AWS / GCP – Hosting & storage

7. Optional (AI / ML)

python, scikit-learn, tensorflow, flask – Smart route optimization
