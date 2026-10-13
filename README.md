# Meine Englisch-App – Version 0.9

## Neu: 🎧 Wörter und Beispielsätze anhören

Im Hörtraining werden zu jedem Wort nicht nur das englische Wort und die deutsche Bedeutung vorgelesen, sondern auch ein **englischer Beispielsatz und seine deutsche Übersetzung**.

**Hörablauf:** englisches Wort → deutsche Bedeutung → (optional englisches Wort wiederholen) → englischer Beispielsatz → deutscher Beispielsatz → (optional englischen Satz wiederholen). Die Stimmen sprechen langsamer als üblich und machen kleine Pausen.

- **Beispielsätze vorlesen** ist standardmäßig aktiviert und lässt sich im Hörtraining ausschalten.
- **Englische Wörter und Sätze wiederholen** ist ebenfalls optional.
- Für **alle 500 vorhandenen Lernwörter** sind jeweils ein englischer Beispielsatz und eine deutsche Übersetzung hinterlegt.
- Bei **selbst eingetragenen Wörtern** liest die App zuerst deine gespeicherten eigenen Beispielsätze. Gibt es keinen solchen Satz, nimmt sie einen passenden vorhandenen Beispielsatz aus der 500-Wörter-Liste, wenn englisches Wort und deutsche Bedeutung übereinstimmen.
- Für andere, selbst eingegebene Wörter ohne Beispielsatz gibt es nur einen **einfachen allgemeinen Übungssatz** („Today I'm learning the word …“ / „Heute lerne ich das Wort …“). Die App erfindet offline *keinen grammatisch oder inhaltlich ungeprüften Kontextsatz*. **Wenn du einen natürlichen Beispielsatz möchtest, kannst du ihn unter „Meine Vokabeln“ auf Englisch und Deutsch hinzufügen.**
- Vorlesen geschieht **lokal über die Stimmen deines iPhones**, ohne KI-Server oder Anmeldung.
- Auswählbare Listen: bisher gelernte Wörter, heute gelernte Wörter, eigene Wörter, alle 500. Steuerung: Start/Pause/Weiter/Stopp/Vorheriges/Nächstes.
- **Wichtig für iPhone:** iOS/Safari kann die Sprachausgabe bei gesperrtem Display oder im Hintergrund anhalten. Lasse die App geöffnet und den Bildschirm eingeschaltet. Es müssen ggf. eine englische und eine deutsche Stimme auf dem Gerät verfügbar sein.

## Bestehende Funktionen und Daten

- 500 englische Wörter (hauptsächlich A1, auch frühes A2) mit deutscher Übersetzung und Beispielsätzen.
- Mindestens 12 Wörter pro Übungsrunde, danach optional weiterlernen.
- Eigene Vokabeln, deutsche/englische Sätze, Training und Sicherungsfunktion bleiben erhalten.
- Die bisherigen lokalen Speicherschlüssel sind unverändert; bestehende Wortlisten und Lernfortschritt bleiben bei einem Update unter **derselben Website-Adresse** erhalten. Datensicherung vor dem Update empfohlen.
- Import unterstützt Sicherungen von v0.6, v0.7 und v0.8. Die neue App exportiert weiterhin das kompatible v0.8-Format, da das gespeicherte Datenschema unverändert ist.

## In GitHub Pages aktualisieren

1. In der bisherigen App unter „Meine Vokabeln“ eine **Sicherung herunterladen**.
2. ZIP-Datei entpacken und **`index.html`, `sw.js`, `manifest.webmanifest`** (und optional `README.md`) in dein **bisheriges GitHub-Repository** hochladen; vorhandene Dateien am selben Ort ersetzen.
3. Auf **Commit changes** klicken und die Aktualisierung abwarten.
4. Die bestehende App auf dem iPhone schließen und neu öffnen. Unten muss **Version 0.9 · 500 Vokabeln** stehen. Bei einer alten Anzeige dieselbe GitHub-Pages-Adresse in Safari neu laden.
5. **Keine Safari-Website-Daten löschen**, keine neue App-Adresse verwenden; dadurch können deine gespeicherten Wörter und der Fortschritt sonst verloren gehen.

## Tests

Die 500 Vokabeleinträge sind auf das Vorhandensein englischer und deutscher Beispielsätze geprüft. JavaScript-Syntaxkontrolle und simulierte Browser-Funktionstests erfolgreich: Reihenfolge der englischen und deutschen Wort-/Satz-Ausgabe, Wiederholen an/aus, Satz-Ausgabe an/aus, eigene gespeicherte Sätze, passende Sätze aus der Wörterliste, Fallback-Satz, Unterbrechen und Weitersteuern sowie Erhalt der bisherigen Speicherschlüssel. **Kein direkter Test auf einem iPhone/Safari** durchgeführt.
