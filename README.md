# Mateen Nawaz — Senior iOS Developer

**6 years · Swift · SwiftUI · UIKit · MVVM · Swift Testing**

I build and own production iOS apps, mostly for clients in Denmark and Greenland: identity and access (Danish MitID, NFC door unlocking for unmanned stores), payments, and telemedicine. I'm the sole iOS engineer at Software Alliance, where I also mentor the company's Android developer.

📍 Lahore, Pakistan
📧 mateennawaz7@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/mateen-nawaz-ios-app-developer)

---

## Software Alliance · 2024 – present

---

### SmartShop 24-7 — New SwiftUI App for Unstaffed Grocery Stores
*Software Alliance · In development*

The next version of the app for SmartShop 24-7, a chain of unstaffed, self-service grocery stores in Denmark that are open around the clock. Customers verify their identity, unlock the store door, find stores, join events and keep their receipts.

**Technical highlights:**
- Built entirely in SwiftUI and Swift 6, using `@Observable` state and value-based `NavigationStack` routing
- Identity verification with MitID (Danish national digital ID) or an ID document plus phone/email OTP
- NFC and in-app door unlock once a customer is verified
- Protocol-based services injected from a single composition root, so each service can run against the live API or an in-memory demo backend
- Migrating from a legacy backend to a new REST API, with Keychain token storage and automatic token refresh
- Danish, English and German, with server-side text overrides
- Unit tests in Swift Testing and UI tests in XCTest

**Tech:** Swift 6 · SwiftUI · async/await · Swift Package Manager · REST APIs · Keychain · NFC · Swift Testing · XCTest

---

### WorcX — Job Management for Trade Businesses
*Software Alliance · For a Danish client · In development*

An app for craftsmen and small trade businesses that runs a job from site inspection to pricing, offer and invoice.

**Technical highlights:**
- One app, two roles (owner and employee): the role comes from the server at login, and screens switch features on or off rather than being duplicated
- Every API call follows the same layered pattern (Endpoint → Resource → ViewModel → ViewController) with async/await
- Features unlock by subscription plan, with Stripe for payment
- Danish and English, with backend-served texts and Danish currency formatting in both languages
- AI-written inspection notes, and a hands-free AI voice assistant (in progress)
- Push notifications that open the right screen
- Swift Testing suite: pure logic tests, ViewModel tests with mocked dependencies, and URLProtocol network stubs

**Tech:** Swift · UIKit · Storyboards · MVVM · async/await · Stripe · Firebase (FCM) · Swift Testing

---

### Safetii Patron — Nightlife Identity Verification
*Software Alliance · [Download on App Store](https://apps.apple.com/pk/app/safetii-patron/id6743107798)*

A digital identity passport for nightlife venues in Denmark.

**Technical highlights:**
- MitID (Danish national digital ID) sign-up through Criipto
- QR code generation with 24-hour expiry for venue access
- Push notifications for incident alerts and access restrictions
- Visit history with check-in and quarantine records

**Tech:** Swift · UIKit · MVVM · Criipto · Firebase (FCM, Auth) · REST APIs · async/await

---

### Safetii Guard — Venue Security App
*Software Alliance · [Download on App Store](https://apps.apple.com/us/app/safetii-guard/id6743107664)*

The companion app for security staff: verify guests, monitor occupancy and manage incidents.

**Technical highlights:**
- QR code scanning to verify a guest's identity against the live backend
- Real-time occupancy monitoring with push-driven updates
- Incident reporting and temporary bans with duration and reason tracking

**Tech:** Swift · UIKit · MVVM · Firebase (FCM) · REST APIs

---

### Pisiffik — Grocery Shopping and Delivery
*Software Alliance · [Download on App Store](https://apps.apple.com/pk/app/pisiffik/id1637092101)*

A shopping and delivery app for a Greenlandic retail chain.

**Technical highlights:**
- Product catalogue, cart management and order tracking
- Digital loyalty membership card: customers earn points on both in-store and in-app purchases
- Checkout across several payment providers, including QuickPay: the server supplies the payment URLs, the app opens them in a WKWebView and confirms success from the response
- Push notifications for order status and promotions

**Tech:** Swift · UIKit · MVVM · WKWebView · Firebase (FCM) · REST APIs

---

### LM Walk-in Vending — Unmanned Warehouse Access
*Software Alliance · [Download on App Store](https://apps.apple.com/pk/app/lm-walk-in-vending/id6746488515)*

A B2B access app for Lemvigh-Müller's unmanned SmartWarehouse locations in Denmark.

**Technical highlights:**
- Secure entry with automatic digital invoicing on exit
- Built for trade customers, with no staff on site
- Lean UIKit implementation with minimal dependencies and careful handling of offline edge cases

**Tech:** Swift · UIKit · MVVM · NFC · REST APIs

---

### Unlimit Key & Smart Shop 24-7 — Shop Access
*Software Alliance · [Unlimit Key](https://apps.apple.com/us/app/unlimit-key/id6476619223) · [Smart Shop 24-7](https://apps.apple.com/pk/app/smart-shop-24-7/id6737332516)*

Find nearby shops and unlock their doors from your phone.

**Technical highlights:**
- NFC door unlock with hardware integration
- MitID sign-up through Criipto
- Google Maps for shop discovery and navigation
- Opening-hours awareness and zip-code search
- English and German

**Tech:** Swift · UIKit · MVVM · NFC · Criipto · Google Maps · Firebase (FCM) · REST APIs

---

### AllahuAlam — Islamic Reference App
*Software Alliance · [Download on App Store](https://apps.apple.com/pk/app/allahualam/id6742174395)*

Quran, prayer times, Qibla direction and reminders in one app.

**Technical highlights:**
- Core Location and Core Motion for accurate prayer times and a Qibla compass
- Audio playback for Quran recitation, synced with translations in several languages
- Stripe payments for the premium tier
- Scheduled push reminders for prayer times

**Tech:** Swift · UIKit · MVVM · Core Location · Core Motion · Stripe · WebSockets · Firebase (FCM, Auth) · REST APIs

---

## Xeven Solutions · 2020 – 2024

---

### Medical AI — Telemedicine Platform
*Xeven Solutions*

A telemedicine app with separate patient and doctor experiences: video consultations, real-time messaging and AI-assisted triage.

**Technical highlights:**
- OpenTok (Vonage) video consultations with in-call SOAP note capture
- Socket.IO patient–doctor messaging with read receipts
- AI chatbot for preliminary symptom triage
- DGCharts analytics dashboard for doctors (patients, earnings, appointments)
- Stripe subscriptions for family plans

**Tech:** Swift · UIKit · MVVM · OpenTok · Socket.IO · Stripe · Firebase · DGCharts · REST APIs

---

### Intely Health — Virtual Healthcare Platform
*Xeven Solutions*

A virtual healthcare app connecting patients with doctors for appointments, video calls and health records.

**Technical highlights:**
- OpenTok video consultations with in-call vitals and SOAP note documentation
- Interactive human-anatomy module so patients can point to where it hurts
- Family subscriptions: several members under one Stripe account
- Secure messaging with file attachments
- Doctor profiles with credentials and educational posts

**Tech:** Swift · UIKit · MVVM · OpenTok · Socket.IO · Stripe · Firebase · REST APIs

---

### Trough — Events and Food-Truck Booking
*Xeven Solutions · [Download on App Store](https://apps.apple.com/us/app/trough/id6443418603)*

Social event planning with food-truck booking, menu ordering and a companion app for drivers.

**Technical highlights:**
- Two apps: one for users and a dedicated one for food-truck drivers
- Stripe payments for event bookings and food orders
- Google Maps for food-truck discovery and live location
- Real-time order updates with push notifications
- Social layer: likes, comments and event feeds

**Tech:** Swift · UIKit · MVVM · Stripe · Google Maps · Firebase (FCM) · REST APIs

---

### Fibra — Digital Receipts
*Xeven Solutions*

Paperless receipts: each user has a personal code, and receipts arrive in the app instantly.

**Technical highlights:**
- Per-user QR code that stores scan to send receipts to the right customer
- Push notifications when a new receipt arrives
- Receipt history stored in Firebase

**Tech:** Swift · UIKit · Firebase (FCM, Firestore) · REST APIs

---

## Skills

| Area | Technologies |
|------|-------------|
| Languages & UI | Swift (incl. Swift 6), SwiftUI (`@Observable`, `NavigationStack`), UIKit (Storyboards, Auto Layout), localization (Danish, English, German) |
| Architecture & concurrency | MVVM, protocol-based services with dependency injection, async/await, Swift 6 strict concurrency, GCD |
| Payments | Stripe (payments and subscription plans), QuickPay and other providers via WKWebView checkout |
| Identity & access | MitID (Criipto), ID-document and OTP verification, NFC, QR codes, Keychain |
| Backend & real-time | REST APIs, Supabase, Firebase (FCM, Firestore, Auth), Socket.IO, WebSockets, OpenTok |
| Location & maps | Google Maps, Core Location, Core Motion |
| Testing & tooling | Swift Testing, XCTest (unit and UI), Swift Package Manager, TestFlight, Git (Bitbucket), Instruments, Jira, Figma |
