<div align="center">

<img src="./assets/cover.svg" alt="Moltaqa Live case study" width="100%"/>

![Source](https://img.shields.io/badge/Source-private-64748b?style=for-the-badge&logo=lock&logoColor=white)

</div>

> 🔒 **The source code is private** (production / client work). This repository is a case study: what the product does, how it is built, and my role. A code walkthrough is available on request: [abdelqader.pro](https://abdelqader.pro) · [LinkedIn](https://www.linkedin.com/in/abdelqader-al-omari/).

## Overview
**Moltaqa Live** ("see it, negotiate, sell") brings real-estate viewing into live video: agents stream properties, buyers
chat in real time, request catalogs and book private tours, all in Arabic and English, on iOS and Android.

## Key features
- 📡 **Live video streaming** with viewer counts and a pinned **property card** ("book a private tour")
- 💬 **Real-time community chat** during every stream, with catalog requests
- ✅ **Verified merchants**: license / commercial-register verification reviewed by admins, so buyers know who they deal with
- 🔐 **Privacy by default**: phone numbers masked unless the user chooses to show them
- 🛡️ **Moderation dashboard**: stream and chat controls, **auto-blocked toxic / spam messages**, user reports, stream scheduling
- 🌍 **Bilingual** Arabic / English

## Architecture

```mermaid
flowchart LR
    B([📱 Buyers]) --> APP[💙 Flutter app<br/>iOS & Android]
    A([🏠 Agents]) --> APP
    APP -->|video| AG[📡 Agora RTC]
    APP -->|chat · profiles| RTDB[(🔥 Firebase Realtime DB<br/>security rules)]
    APP --> CF[☁️ Cloud Functions]
    CF -->|secure stream tokens| AG
    ADM([🛡️ Admins]) --> APP
```

## My role
Mobile and backend development: the Flutter app, Firebase data model and security rules, Cloud Functions for secure
stream tokens, moderation tooling, and store-release preparation.

## Tech
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white) ![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black) ![Agora RTC](https://img.shields.io/badge/Agora_RTC-099DFD?style=for-the-badge&logo=livestream&logoColor=white) ![Cloud Functions](https://img.shields.io/badge/Cloud_Functions-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)

## Screenshots

<p align="center"><img src="./assets/feature.jpg" alt="Moltaqa Live" width="100%"/></p>

<table><tr><td align="center" width="25%"><img src="./assets/live.jpg" alt="Live stream with property card and chat" width="100%"/><br/><sub>Live stream with property card and chat</sub></td><td align="center" width="25%"><img src="./assets/profile.jpg" alt="Profile with verified merchant mode" width="100%"/><br/><sub>Profile with verified merchant mode</sub></td><td align="center" width="25%"><img src="./assets/verification.jpg" alt="Merchant license verification" width="100%"/><br/><sub>Merchant license verification</sub></td><td align="center" width="25%"><img src="./assets/admin.jpg" alt="Admin moderation dashboard" width="100%"/><br/><sub>Admin moderation dashboard</sub></td></tr></table>

---

<div align="center">

**Built by [Abdelqader Al-Omari](https://github.com/abdelqader-alomari)** · Senior Full-Stack Engineer · AI & Enterprise Solutions

[![Portfolio](https://img.shields.io/badge/abdelqader.pro-8b5cf6?style=for-the-badge&logo=googlechrome&logoColor=white)](https://abdelqader.pro) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdelqader-al-omari/) [![More work](https://img.shields.io/badge/More_case_studies-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdelqader-alomari)

</div>
