# xp-farmers / Rite of Reflex (Universitätsprojekt – Sommersemester 2025)

Ein im Rahmen des Kurses **„Game Development“** an der **Berliner Hochschule für Technik (BHT)** entwickeltes Spieleprojekt mit **Unity & C#**. 

*Hinweis für Arbeitgeber: Aufgrund von LFS-Infrastrukturänderungen des universitären Git-Servers ist der Quellcode inklusive der vollständigen, originalen **232 Commit-Nachrichten (als Entwicklungsnachweis)** auf Anfrage jederzeit als ZIP-Archiv verfügbar.*

---

## Meine Rolle & Technische Umsetzung
Ich habe den **Großteil der Software-Architektur und Kern-Systeme** des Spiels übernommen. Mein Fokus lag auf dem Entwurf modularer, objektorientierter Strukturen (OOP) und sauberer Daten-Trennung:

### Architektur-Highlights aus meinem Code:
* **Modulares Kampfsystem (`Weapon` & `WeaponData`):** Strikt datengetriebener Ansatz. Waffen-Logik (`Weapon`) und veränderbare Waffen-Werte (Skriptfähige Objekte via `WeaponData`) wurden sauber getrennt, um maximale Flexibilität beim Balancing zu garantieren.
* **Erweiterbares Minispiel-System (`SkillChecks`):** Nutzung einer sauberen Vererbungsstruktur über eine Basisklasse (`SkillCheckBase`), von der spezifische Mechaniken wie das `TimingBarSkillCheck`, `LabyrinthMinigame` oder ein Rhythmus-basiertes `DDRSkillcheck` abgeleitet wurden.
* **Interfaces für lose Kopplung:** Implementierung von `ICombatant` und `IInteractable`, um Interaktionen im Spiel (z. B. mit Türen via `Door`) und Schadensberechnungen flexibel und modular zu halten.
* **Dynamisches UI-Feedback:** Entwicklung des `DamagePopUp System` (inkl. `DamageLabel`), um Kampffeedback visuell sauber vom Gameplay-Code getrennt darzustellen.

### Generative AI als Architektur-Copilot
Bei der Strukturierung dieser komplexen Systeme und der Entscheidung über den saubersten Aufbau von Klassenbeziehungen habe ich **generative KI-Tools (z. B. ChatGPT)** gezielt als Sparringspartner genutzt.
* **Einsatzbereich:** Validierung von OOP-Architekturen, Diskussion über lose Kopplung via Interfaces und Code-Refactoring für optimale Lesbarkeit (Clean Code).
* **Ergebnis:** Eine hochgradig skalierbare Codebasis, die im Teamprojekt die Grundlage für den gesamten Gameplay-Loop bildete.

---

## Tech-Stack
* **Engine:** Unity 
* **Sprache:** C# (OOP, Interfaces, Scriptable Objects)
* **Kollaboration:** Git / GitLab (232 Commits im Teamverlauf)
