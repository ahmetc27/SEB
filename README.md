# SWEN1 Sports Exercise Battle (SEB)

Eine Webanwendung mit sauberer Schichtarchitektur für die Verwaltung von Sportbattles und Turnieren, entwickelt im Rahmen der Lehrveranstaltung **SWEN1**.

## 📌 Projektbeschreibung

Die Sports Exercise Battle (SEB) Anwendung ermöglicht es Benutzern, an virtuellen Sportbattles teilzunehmen und ihre Fähigkeiten in Turnieren unter Beweis zu stellen. Das System verwaltet Benutzerprofile, Sessions, Statistiken und bietet ein ausgeklügeltes Ranking-System.

### 🎯 Unique Feature: Elo-basiertes Ranking-System
Das Herzstück der Anwendung ist ein **dynamisches Ranking-System** basierend auf Elo-Werten. Spieler steigen basierend auf ihrer Performance in verschiedene Ränge auf:
- Bronze (< 1200 Elo)
- Silber (1200-1599 Elo) 
- Gold (1600-1999 Elo)
- Platin (2000+ Elo)

## 🏗️ Architektur

Das Projekt folgt einer **Clean Architecture** mit klarer Trennung der Verantwortlichkeiten:

- **Controller** – HTTP-Request-Verarbeitung und Response-Generierung
- **Services** – Business-Logik, Validierung und Datenverarbeitung
- **Repositories** – Datenzugriff und Persistierung
- **Models/DTOs** – Datenstrukturen und Transfer-Objekte
- **Exceptions** – Einheitliche Fehlerbehandlung

## ✨ Features

- 👤 **Benutzerverwaltung** – Registrierung, Authentifizierung und Profilmanagement
- 🎮 **Session-Management** – Sichere Benutzer-Sessions
- 📊 **Statistik-System** – Detaillierte Performance-Metriken
- 🏆 **Turnierverwaltung** – Organisation und Durchführung von Wettkämpfen
- 📈 **Elo-Ranking** – Dynamisches Bewertungssystem
- 📋 **Battle-History** – Vollständige Aufzeichnung aller Matches
- 🚨 **Robuste Fehlerbehandlung** – Konsistente Exception-Behandlung

## 🛠 Technologie-Stack

- **Backend:** C# (.NET 6/7)
- **Testing:** NUnit Framework
- **Architektur:** Clean Architecture Pattern
- **Datenbank:** [Bitte spezifizieren falls verwendet]

## 📂 Projektstruktur

```
SEB/
├── Controllers/        # HTTP-Endpunkt-Handler
├── Services/          # Business-Logic-Layer
├── Repositories/      # Data-Access-Layer
├── Models/           # Domain-Modelle
├── Dtos/             # Data-Transfer-Objects
├── Interfaces/       # Service-Contracts
├── Mappers/          # Object-Mapping-Logic
├── Exceptions/       # Custom-Exception-Classes
├── Http/             # HTTP-Utilities
├── Utils/            # Helper-Functions
└── Program.cs        # Application-Entry-Point
```

## 🧪 Umfassende Testsuite

Das Projekt verfügt über **60+ NUnit-Tests** mit einer Abdeckung aller kritischen Komponenten:

- **User-Tests** – Registrierung, Login, Profilmanagement
- **Session-Tests** – Authentifizierung und Session-Handling  
- **Stats-Tests** – Statistik-Berechnung und Ranking-Algorithmus
- **Tournament-Tests** – Turnier-Logic und Matchmaking
- **History-Tests** – Battle-Aufzeichnung und -Abruf

### Test-Kategorien:
- ✅ **Positive Tests** – Korrekte Funktionalität
- ❌ **Negative Tests** – Fehlerbehandlung und Edge-Cases
- 🏆 **Ranking-Tests** – Elo-System-Validierung

## 🚀 Installation & Setup

### Voraussetzungen
- .NET 6 oder höher
- Git

### Schritt-für-Schritt Installation

1. **Repository klonen:**
   ```bash
   git clone https://github.com/ahmetc27/FHTW_SWEN1_SEB.git
   cd FHTW_SWEN1_SEB
   ```

2. **Dependencies installieren:**
   ```bash
   dotnet restore
   ```

3. **Anwendung starten:**
   ```bash
   dotnet run
   ```

4. **Tests ausführen:**
   ```bash
   dotnet test
   ```

### Konfiguration
[Hier können spezifische Konfigurationsschritte ergänzt werden, falls erforderlich]

## 📈 API-Endpunkte

Die Anwendung stellt folgende Hauptendpunkte bereit:

- `/api/users` - Benutzerverwaltung
- `/api/sessions` - Session-Handling  
- `/api/stats` - Statistiken und Rankings
- `/api/tournaments` - Turnierverwaltung
- `/api/history` - Battle-Verlauf

[Detaillierte API-Dokumentation kann hier verlinkt oder erweitert werden]

## 🎯 Entwicklungsaufwand

**Gesamtaufwand:** ~60-70 Stunden
- Architektur & Setup: 10h
- Feature-Entwicklung: 35h
- Testing & QA: 15h
- Dokumentation: 5h

## 🤝 Beitrag & Entwicklung

Dieses Projekt wurde als Einzelarbeit im Rahmen der SWEN1-Lehrveranstaltung entwickelt und demonstriert die praktische Anwendung von Clean Architecture Prinzipien.
