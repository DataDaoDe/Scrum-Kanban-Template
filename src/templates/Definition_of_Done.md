# Definition of Done (DoD)

Die Definition of Done (DoD) legt die Kriterien fest, die eine Story oder ein Backlog-Item erfüllen muss, um als "fertig" betrachtet zu werden. Dies stellt sicher, dass alle Aufgaben vollständig abgeschlossen sind und keine Arbeiten mehr offen bleiben.


## **Definition of Done (DoD) Template**

#### **1. Allgemeine Anforderungen**
- [ ] **Akzeptanzkriterien erfüllt**: Alle Akzeptanzkriterien des Tickets sind erfüllt und überprüft.
- [ ] **Funktionalität implementiert**: Die geforderte Funktionalität ist vollständig implementiert und funktioniert wie erwartet.
- [ ] **Keine bekannten Fehler**: Es sind keine bekannten kritischen oder schwerwiegenden Fehler vorhanden.

#### **2. Code-Qualität**
- [ ] **Code-Reviews durchgeführt**: Der Code wurde von mindestens einem anderen Teammitglied überprüft und genehmigt.
- [ ] **Coding-Standards eingehalten**: Der Code entspricht den definierten Coding-Standards und Best Practices.
- [ ] **Keine technischen Schulden**: Technische Schulden wurden vermieden oder dokumentiert, und es gibt keine offenen Aufgaben, die die Code-Qualität beeinträchtigen.

#### **3. Tests**
- [ ] **Unit Tests vorhanden**: Alle neuen Funktionen sind durch Unit Tests abgedeckt.
- [ ] **Integration Tests erfolgreich**: Falls relevant, wurden Integration Tests durchgeführt und bestanden.
- [ ] **Manuelle Tests durchgeführt**: Manuelle Tests wurden durchgeführt, um sicherzustellen, dass die Funktionalität den Erwartungen entspricht.

#### **4. Dokumentation**
- [ ] **Benutzerdokumentation aktualisiert**: Falls notwendig, wurde die Benutzerdokumentation oder die Benutzeranleitung aktualisiert.
- [ ] **Technische Dokumentation aktualisiert**: Die technische Dokumentation oder das Wiki wurde aktualisiert, um die Änderungen widerzuspiegeln.
- [ ] **Release Notes hinzugefügt**: Wichtige Änderungen oder neue Funktionen sind in den Release Notes dokumentiert.

#### **5. Integration und Deployment**
- [ ] **Branch in das Haupt-Repository integriert**: Der Code wurde erfolgreich in den Hauptentwicklungsbranch (z.B. `main` oder `develop`) integriert.
- [ ] **Continuous Integration (CI) erfolgreich**: Alle CI-Pipelines (Build, Tests, etc.) wurden erfolgreich abgeschlossen.
- [ ] **Staging-Umgebung bereitgestellt**: Die Änderungen wurden in der Staging-Umgebung bereitgestellt und getestet.
- [ ] **Keine Merge-Konflikte**: Alle Merge-Konflikte wurden gelöst.

#### **6. Produktqualität und Akzeptanz**
- [ ] **Akzeptanz durch Product Owner**: Der Product Owner hat die Arbeit überprüft und akzeptiert.
- [ ] **Feedback berücksichtigt**: Eventuelles Feedback vom Product Owner oder Stakeholdern wurde eingearbeitet.

#### **7. Sicherheit und Compliance**
- [ ] **Sicherheitsüberprüfungen durchgeführt**: Falls zutreffend, wurden Sicherheitsüberprüfungen durchgeführt und bestanden.
- [ ] **Compliance-Anforderungen erfüllt**: Alle relevanten Compliance- oder rechtlichen Anforderungen wurden berücksichtigt.

#### **8. Performance**
- [ ] **Performance überprüft**: Die Performance wurde getestet und ist innerhalb akzeptabler Grenzen.
- [ ] **Keine Beeinträchtigung der Systemstabilität**: Es wurde sichergestellt, dass die Änderungen keine negativen Auswirkungen auf die Stabilität des Systems haben.

#### **9. Benutzerfreundlichkeit**
- [ ] **UI/UX-Kriterien erfüllt**: Falls zutreffend, entsprechen die Änderungen den festgelegten Benutzerfreundlichkeits- und UX-Anforderungen.