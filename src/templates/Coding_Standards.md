# Coding Standards

### **Best Practices und Coding Standards Template**

#### **1. Allgemeine Coding Prinzipien**

##### **1.1. Lesbarkeit**
- [ ] **Klarer und aussagekräftiger Code**: Schreibe den Code so, dass er leicht verständlich ist, sowohl für aktuelle Teammitglieder als auch für zukünftige Entwickler.
  - Verwende sprechende Variablen- und Funktionsnamen (z.B. `calculateTotalPrice` statt `calc`).
  - Schreibe kurze und klare Kommentare, die erklären, warum etwas gemacht wird (nicht nur was gemacht wird).
  - Verwende Codeformatierungstools (z.B. Prettier, Black), um eine einheitliche Struktur zu gewährleisten.
- [ ] **Konventionen befolgen**: Halte dich an die im Team definierten Coding-Konventionen (z.B. Namenskonventionen, Code-Style).
  - Beispiel: Für JavaScript/TypeScript kann ESLint verwendet werden, für Python PEP 8.

##### **1.2. Wartungsfähigkeit**
- [ ] **Modularer Code**: Teile deinen Code in kleine, wiederverwendbare und unabhängige Module auf.
  - Eine Funktion sollte nur eine einzige Aufgabe haben (Single Responsibility Principle).
  - Vermeide lange Funktionen oder Methoden – strebe nach Funktionen mit maximal 20-30 Zeilen.
- [ ] **Code-Duplizierung vermeiden (DRY-Prinzip)**: Vermeide es, denselben Code an mehreren Stellen zu schreiben.
  - Verwende Funktionen, Module und Klassen, um häufig verwendete Logik auszulagern.
  - Beispiel: Statt wiederholter Validierungen an verschiedenen Stellen, eine zentrale Validierungsfunktion erstellen.
  
##### **1.3. Effizienz**
- [ ] **Effiziente Algorithmen**: Wähle Algorithmen und Datenstrukturen, die eine hohe Effizienz hinsichtlich Zeit und Speicher bieten.
  - Verwende z.B. O(n) Algorithmen, wo immer möglich, und vermeide ineffiziente O(n^2) Operationen in großen Schleifen.
  - Beispiel: Verwende HashMaps/Dictionaries für schnelle Suchen statt linearer Suchen in Arrays.
- [ ] **Ressourcenmanagement**: Achte auf den bewussten Umgang mit Speicher, Netzwerkressourcen und Dateien.
  - Verwende z.B. Lazy-Loading oder Pagination bei großen Datenmengen, um Ressourcen effizient zu nutzen.
  - Schließe geöffnete Ressourcen wie Datenbankverbindungen oder Dateien korrekt (z.B. mit `with`-Statements in Python).

##### **1.4. Zuverlässigkeit**
- [ ] **Fehlerbehandlung**: Verwende robuste Fehlerbehandlung, um den Code vor unerwarteten Abstürzen zu schützen.
  - Beispiel: Verwende Try-Catch-Blöcke für mögliche Fehler und gebe aussagekräftige Fehlermeldungen aus.
  - Schreibe Tests, um sicherzustellen, dass Fehlerfälle abgedeckt sind (Unit Tests, Integrationstests).
- [ ] **Edge Cases berücksichtigen**: Denke an Grenzfälle und potenziell fehlerhafte Eingaben.
  - Beispiel: Was passiert, wenn eine leere Liste oder null/undefined übergeben wird?
  
##### **1.5. Wiederverwendbarkeit**
- [ ] **Wiederverwendbare Komponenten**: Schreibe Code, der für mehrere Projekte oder Anwendungen verwendet werden kann.
  - Beispiel: Bibliotheken oder Module, die unabhängig von der spezifischen Anwendung sind.
- [ ] **Parametrisierbare Funktionen und Klassen**: Verwende Parameter, um Funktionen flexibel und wiederverwendbar zu gestalten.
  - Beispiel: Schreibe eine allgemeine Sortierfunktion, die verschiedene Vergleichsoperationen akzeptiert.
  
---

#### **2. Struktur und Organisation des Codes**

##### **2.1. Projektstruktur**
- [ ] **Klar definierte Verzeichnisse**: Organisiere den Code in gut strukturierten Verzeichnissen nach Funktionen oder Komponenten.
  - Beispiel: Verwende Verzeichnisse wie `src`, `tests`, `config`, `utils`, und `components`.
  - Trenne Business-Logik, Datenzugriffslogik und Benutzeroberfläche in separaten Schichten (Schichtarchitektur).
  
##### **2.2. Code-Dokumentation**
- [ ] **Dokumentation des Codes**: Füge zu komplexem Code aussagekräftige Dokumentationen hinzu (z.B. mit Tools wie JSDoc, Sphinx).
  - Stelle sicher, dass jede Funktion, Klasse und jedes Modul klar dokumentiert ist, mit Erklärungen der Eingaben, Ausgaben und des Verhaltens.
  
##### **2.3. Versionskontrolle**
- [ ] **Branching-Strategie**: Verwende eine standardisierte Branching-Strategie (z.B. Git Flow, Feature Branches) für saubere Versionskontrolle.
  - Beispiel: Nutze `main` oder `master` für stabile Versionen und `develop` für laufende Entwicklung.
- [ ] **Kleine, gut definierte Commits**: Mache regelmäßig kleine und fokussierte Commits, die eine einzelne Änderung oder Verbesserung beinhalten.

---

#### **3. Tests und Qualitätssicherung**

##### **3.1. Unit Tests**
- [ ] **Schreibe Unit Tests für jede Funktion**: Teste jede kleine Komponente isoliert, um sicherzustellen, dass sie korrekt funktioniert.
  - Beispiel: Verwende Tools wie PyTest für Python oder Jest für JavaScript.
  
##### **3.2. Integrationstests**
- [ ] **Teste die Zusammenarbeit von Modulen**: Stelle sicher, dass die Module und Komponenten nahtlos zusammenarbeiten.
  - Beispiel: Schreibe Integrationstests für End-to-End Flows, wie z.B. Benutzerregistrierung und -login.

##### **3.3. Testabdeckung**
- [ ] **Hohe Testabdeckung anstreben**: Strebe eine Testabdeckung von mindestens 80% an, ohne sich nur auf die Quantität zu fokussieren.
  - Teste kritische Pfade und Edge Cases gründlich.

##### **3.4. Automatisiertes Testen und Continuous Integration**
- [ ] **Automatisierte Tests verwenden**: Implementiere Continuous Integration (CI)-Pipelines, um automatisch Tests bei jedem Commit oder Merge auszuführen (z.B. mit Jenkins, GitHub Actions).
  - Beispiel: Alle Tests müssen in der Pipeline bestehen, bevor Code in den Hauptbranch gemergt werden darf.

---

#### **4. Best Practices für Code-Optimierung**

##### **4.1. Refactoring**
- [ ] **Kontinuierliches Refactoring**: Verbessere regelmäßig den Code, um Redundanzen zu entfernen und die Lesbarkeit zu erhöhen.
  - Beispiel: Funktionen, die ähnliche Aufgaben erfüllen, zu einer allgemeinen Funktion kombinieren.
  
##### **4.2. Keine „Magic Numbers“ oder „Hardcoding“**
- [ ] **Vermeide Magic Numbers**: Vermeide es, Zahlen direkt in den Code zu schreiben, ohne sie zu benennen oder zu erklären.
  - Beispiel: Verwende Konstanten wie `MAX_RETRIES = 3` anstelle von `if retries < 3`.

##### **4.3. Optimierung von Datenbank- und Netzwerkaufrufen**
- [ ] **Datenbankabfragen optimieren**: Verwende effiziente Datenbankabfragen und Indexe, um Performance zu verbessern.
  - Beispiel: Vermeide das Abrufen großer Datenmengen, wenn nur wenige Zeilen benötigt werden (Paging nutzen).
  
##### **4.4. Asynchrone Programmierung**
- [ ] **Asynchronität für bessere Performance**: Verwende asynchrone Operationen (z.B. `async/await` in JavaScript), um parallele Aufgaben wie API- oder Datenbankaufrufe zu optimieren.
  - Beispiel: Parallelisiere langlaufende Aufgaben, um die Ausführungszeit zu reduzieren.

---

#### **5. Sicherheit**

##### **5.1. Input-Validierung**
- [ ] **Sanitisiere und validiere Benutzereingaben**: Schütze den Code vor Angriffen wie SQL-Injections oder XSS durch ordnungsgemäße Validierung und Sanitisierung von Eingaben.
  - Beispiel: Verwende Parameterized Queries für SQL und Escape-Sequenzen für HTML.

##### **5.2. Fehler sicher behandeln**
- [ ] **Sichere Fehlerbehandlung**: Vermeide das Ausgeben von detaillierten Fehlermeldungen an den Benutzer, um keine sensiblen Informationen preiszugeben.
  - Beispiel: Bei einem API-Fehler sollte nur eine allgemeine Fehlermeldung zurückgegeben werden, keine Details zur internen Struktur.

##### **5.3. Authentifizierung und Autorisierung**
- [ ] **Sichere Authentifizierung**: Verwende bewährte Verfahren wie OAuth 2.0 oder JWT für Authentifizierung.
- [ ] **Zugriffskontrollen implementieren**: Stelle sicher, dass Benutzer nur auf Ressourcen zugreifen, für die sie autorisiert sind.