# Trainiq.

> Krafttraining, Cardio, Ernährung. Editorial gestaltet, spürbar privat.

Eine iOS-App für Menschen, die ihr Training ernst nehmen — aber keine Lust auf Werbung, Pop-ups und Daten­sammeln haben. Sätze, Pausen, Pace, Mahl­zeiten, alles auf einem Gerät, alles unter deiner Kontrolle.

---

## Inhalt

- [Was Trainiq macht](#was-trainiq-macht)
- [Funktionen](#funktionen)
  - [Krafttraining](#krafttraining)
  - [Ernährung & Kochbuch](#ernährung--kochbuch)
  - [Cardio & GPS](#cardio--gps)
  - [KI-Coach](#ki-coach)
  - [Apple Watch & Live Activity](#apple-watch--live-activity)
- [Privatsphäre](#privatsphäre)
- [Stack](#stack)
- [Status](#status)
- [Kontakt](#kontakt)

---

## Was Trainiq macht

Trainiq ist ein **Trainings-Tracker für iPhone und Apple Watch**. Du planst deine Workouts, trackst deine Sätze, speicherst deine Mahl­zeiten und behältst deine Pace im Blick. Alles direkt auf dem Gerät, ohne Konto, ohne Server.

Drei Säulen, eine App:

| Säule | Was passiert | Wo |
|---|---|---|
| **Krafttraining** | Pläne, Sätze, Wiederholungen, Pausen, Supersätze, Drop-Sätze | iPhone &middot; Watch |
| **Ernährung** | Mahlzeiten, Kalorien, Makros, Coach-Vorschläge ins Kochbuch | iPhone |
| **Cardio** | GPS-Tracking für Laufen, Radfahren, HIIT, Schwimmen | iPhone &middot; Watch |

---

## Funktionen

### Krafttraining

Plane Workouts wie du willst — mit normalen Arbeits­sätzen, **Aufwärm­sätzen**, **AMRAP-Sätzen** (so viele Wieder­holungen wie möglich), **Super­sätzen** (zwei Übungen ohne Pause hinter­einander) und **Drop-Sätzen** (Haupt­satz voll, Gewicht runter, sofort weiter).

Während des Trainings:

- Live-Eingabe direkt auf der Übungs-Card. Tippen, eintragen, weiter.
- Pausen-Timer mit **Live Activity** auf dem Sperr­bildschirm und in der **Dynamic Island** — kein App-Wechsel nötig, du siehst die verbleibende Pause im Augen­winkel.
- **1-Tap-Satz-Feedback** (Leicht · Perfekt · Schwer · Versagt) — der Coach lernt damit, wann er dir mehr Gewicht oder Wieder­holungen vorschlägt.
- **Persönliche Notizen pro Übung** — plan­übergreifend. Was du dir bei Bank­drücken merkst, gilt überall wo du Bank­drücken machst.

---

### Ernährung & Kochbuch

Ernährung ist kein Add-on — sie ist eine eigene Säule. Trainiq trackt **Kalorien, Eiweiß, Kohlen­hydrate und Fett pro Tag**, mit einem Editorial-Layout das nicht aussieht wie eine Excel-Tabelle.

Was du machen kannst:

- **Mahl­zeiten loggen** mit Kalorien- und Makro­werten, in einer **Tages­bilanz** die zeigt wo du stehst.
- Den **Coach nach Mahl­zeit­ideen fragen** — *„Was kann ich heute Abend kochen mit 600 kcal und 40 g Eiweiß?"* — und seine Vorschläge direkt mit einem Tap in dein Tages­tracking übernehmen.
- **Kochbuch:** Lieblings­mahl­zeiten als Rezepte speichern und beim nächsten Mal mit einem Tap wieder loggen. Bei Coach-generierten Mahl­zeiten kannst du gleich entscheiden: *„Heute essen"* oder *„Ins Kochbuch für später"*.

> *Kochbuch ist in finaler Entwicklung und kommt mit dem ersten großen Update nach Launch.*

---

### Cardio & GPS

Laufen, Radfahren, HIIT, Schwimmen, Wandern, Walking, Rudern — als eigener Tab mit echten Anatomie-Bildern, nicht den üblichen abstrakten Icons.

- **GPS-Tracking** für Lauf­strecken, Pace und Höhen­meter. Karten­anzeige in den Cardio-Details.
- **Wochen- und Monats­statistik** im Editorial-Layout, plus 30-Tage-Grid mit dem was du wirklich gemacht hast.
- **Lauf­pläne** mit Progress-Ring, vom Coach erstellbar.
- GPS-Daten bleiben **ausschließlich auf dem Gerät** — keine Übertragung an irgendeinen Server.

---

### KI-Coach

Ein optionaler Coach, mit dem du **per Chat** über dein Training und deine Ernährung redest. Er kennt deine letzten Workouts, deine Pläne, deine Maße — soweit du sie eingetragen hast.

Was er kann:

- **Neue Pläne anlegen.** *„Mach mir einen Push-Plan für 3× die Woche, 60 Min."* — er erstellt den Plan direkt in der App, du musst nur bestätigen.
- **Steigerungen vorschlagen.** Auf Basis von Satz-Feedback und Volumen­entwicklung der letzten Wochen.
- **Mahl­zeiten konzipieren.** Anhand deines Tages­ziels und was du heute schon gegessen hast.
- **Lauf­pläne strukturieren** für 5K, 10K oder Halb­marathon.

**Was nicht übermittelt wird:** Name, E-Mail, Standort. Nur Trainings­daten, Übungs­namen und dein Satz-Feedback. Alles über einen eigenen Cloudflare Worker in der EU, von dort weiter an Anthropic.

---

### Apple Watch & Live Activity

Trainiq ist nativ auf **watchOS**, nicht über das iPhone gespiegelt:

- **Active Workout Card** im Editorial-Stil — Übungs­name groß, kg × Wdh prominent, „Satz fertig"-Button.
- **1-Tap-Feedback** (Leicht · Perfekt · Schwer · Versagt) direkt auf der Uhr, ohne Tastatur.
- **Live Activity** auf dem iPhone-Sperr­bildschirm während die Pause läuft.
- **Dynamic Island** zeigt Satz­fortschritt + Pausen-Timer im Live-Modus.

---

## Privatsphäre

Trainiq ist eine der wenigen Fitness-Apps, bei denen das ernst gemeint ist:

| | Trainiq |
|---|---|
| Konto / Anmeldung | Nicht nötig |
| E-Mail beim Setup | Nicht nötig |
| Werbung | Keine |
| Tracker-SDKs | Keine |
| IDFA | Wird nicht erhoben |
| Trainings­daten | Lokal auf dem iPhone (SwiftData) |
| GPS-Routen | Lokal auf dem iPhone |
| Mahl­zeiten | Lokal auf dem iPhone |
| Backup | Nur dein iCloud-Backup, wenn aktiv |
| Coach-Anfragen | Anonymisiert, ohne perso­nen­bezogene Daten |

Volle Daten­schutz­erklärung &rarr; [`datenschutz.html`](datenschutz.html)

---

## Stack

Für die, die es interessiert. Trainiq ist eine **Indie-App von einem einzelnen Entwickler**, gebaut mit Apples eigenen Werk­zeugen. Kein React Native, kein Flutter, kein Frame­work-Bloat.

```
UI            →  SwiftUI
Persistenz    →  SwiftData
Health        →  HealthKit
Wearable      →  watchOS (nativ)
Live          →  ActivityKit · Live Activity · Dynamic Island
Musik         →  MusicKit
Cardio        →  CoreLocation · GPS
Widgets       →  WidgetKit
Minimum       →  iOS 17
```

Backend für Coach-Anfragen: Eigener **Cloudflare Worker** als Proxy, KEIN eigener Daten­bank-Server. Keine User-Konten, keine Datenbank im Hintergrund.

---

## Status

| Phase | Stand |
|---|---|
| **Closed Beta** | TestFlight, internationale Tester &middot; läuft |
| **App-Store-Einreichung** | In Vorbereitung |
| **Public Launch** | Bald |
| **Kochbuch + Meal-Coach** | In finaler Entwicklung |
| **Watch-Phase 2** (Handoff iPhone &rarr; Watch) | Im Backlog |

Wenn du an der Beta teilnehmen willst, schreib eine Mail — Plätze sind begrenzt, aber Anfragen sind willkommen.

---

## Kontakt

**Elbe Studio** &middot; Magdeburg
&rarr; [elbstudio.app@gmail.com](mailto:elbstudio.app@gmail.com)

Für Beta-Anfragen, Bug-Reports, Feature-Wünsche oder einfach Hallo.

---

<sub>© 2026 Elbe Studio</sub>
