# 🌱 AgriFlow – Smart Farming Desktop Application

## Overview

This project was developed as part of the PIDEV – 3rd Year Engineering Program at **Esprit School of Engineering** (Academic Year 2025–2026).

AgriFlow is a JavaFX desktop application designed to digitize and optimize agricultural management in Tunisia. It provides smart, accessible digital tools for farmers, experts, and administrators to manage parcels, crops, marketplaces, diagnostics, irrigation plans, and more.

---
## 🌍 Live Demo
Project website available at:
https://maatougayoub.github.io/Esprit-PIDEV-3A14-2025-2026-AgriFlow/

## Features

### CRUD Operations
| Entity | Operations |
|--------|-----------|
| **Annonces (Listings)** | Create, Read, Update, Delete |
| **Reservations** | Book, View, Cancel |
| **Cultures (Crops)** | Create, Read, Update, Delete |
| **Parcelles (Parcels)** | Create, Read, Update, Delete |
| **Utilisateurs (Users)** | Create, Read, Update, Delete |
| **Produits (Products)** | Create, Read, Update, Delete |
| **Réclamations** | Submit, View, Manage |

### Advanced Business Features
- 🤖 **Gemini AI** — description enhancement, price suggestion, content moderation
- 🛡️ **Anti-fraud detection** — automatic suspicious content detection
- 📄 **PDF Contracts** — automatic generation with iText 7
- ✍️ **Automatic signing** on generated contracts
- 🌿 **AI Diagnostics** — crop disease detection and recommendations
- 💧 **Irrigation Planning** — smart irrigation schedule management
- 🤝 **Collaboration Requests** — expert-farmer collaboration system
- 🛒 **Marketplace** — agricultural product trading platform
- 💳 **Stripe Integration** — online payment processing

### User Roles
- **Farmers (Agriculteurs)**: manage profiles, parcels, crops, diagnostics, marketplace
- **Administrators**: manage users, validate data, monitor the platform
- **Experts**: provide diagnostics, irrigation planning, collaboration with farmers

---

## Tech Stack

### Frontend
| Technology | Usage |
|-----------|-------|
| JavaFX 21 | Graphical user interface |
| FXML | UI layout definition |
| CSS | Styling and theming |
| Scene Builder | UI design tool |

### Backend
| Technology | Usage |
|-----------|-------|
| Java 17 | Core application language |
| MySQL | Relational database |
| JDBC | Database connectivity |
| iText 7 | PDF contract generation |
| Google Gemini API | AI-powered features |
| Stripe API | Payment processing |
| Telegram Bot API | Notifications |
| JUnit 5 | Unit testing |
| Maven | Dependency management |

---

## Architecture

The project follows the **MVC (Model-View-Controller)** pattern:

```
agriflow/
├── src/main/java/
│   ├── controllers/    ← JavaFX Controllers (UI logic)
│   ├── entities/       ← Data models: User, Annonce, Reservation, Culture, Parcelle, etc.
│   ├── services/       ← Business logic: CRUD + AI + Anti-fraud + PDF
│   ├── utils/          ← Utilities: MyDatabase (Singleton), helpers
│   ├── validators/     ← Input validation classes
│   └── mains/          ← AppLauncher entry point
├── src/main/resources/
│   ├── *.fxml          ← JavaFX views
│   ├── styles.css      ← Global stylesheet
│   └── images/         ← Assets and logo
├── src/test/java/      ← JUnit 5 unit tests
├── contrats/           ← Generated PDF contracts
├── uploads/            ← User uploaded files (certifications, logos, etc.)
├── agriflow9 (1).sql   ← Full database script
└── pom.xml             ← Maven configuration
```

---

## Contributors

| Name | Role |
|------|------|
| **Ayoub Maatoug** | Team member — TeamSpark |
| **Oussama Fattoumi** | Team member — TeamSpark |
| **Amenallah Jerbi** | Team member — TeamSpark |
| **Badis Beji** | Team member — TeamSpark |
| **Yakine Sahli** | Team member — TeamSpark |

---

## Academic Context

Developed at **Esprit School of Engineering** – Tunisia

**PIDEV – 3A | 2025–2026**

> Project developed within the framework of the Professional Integration Project (PIDEV) for 3rd year engineering students at **Esprit School of Engineering**.

---

## Getting Started

### Prerequisites
- Java 17+
- MySQL Server + phpMyAdmin
- IntelliJ IDEA (or any Java IDE)
- Maven

### 1. Database Setup
```bash
1. Open phpMyAdmin (http://localhost/phpmyadmin)
2. Import the file: agriflow9 (1).sql  (automatically creates the database and tables)
```

### 2. Run the Application
```bash
1. Open the project in IntelliJ IDEA
2. Build → Rebuild Project
3. Run Configuration → Main class: mains.AppLauncher
4. Click Run
```

### 3. Default Test Account
> Simulated user: **Amenallah Jerbi** (id=39, role=AGRICULTEUR)

---

## Acknowledgments

- [Google Gemini API](https://ai.google.dev/) — AI integration for smart agricultural features
- [iText 7](https://itextpdf.com/) — PDF generation library
- [Stripe](https://stripe.com/) — Payment processing
- [OpenJFX / JavaFX](https://openjfx.io/) — Desktop UI framework
- **Esprit School of Engineering** — Academic supervision and support

